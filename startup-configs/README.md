# Startup Configurations

Configuration files for applications and services that run on system startup.

## 📝 What to Include

- **LaunchAgents**: macOS launch agents and daemons
- **Systemd**: Linux systemd service files
- **Cron Jobs**: Scheduled task configurations
- **Docker**: Docker compose files for development services
- **Environment**: Environment setup scripts

## 📂 Suggested Organization

```
startup-configs/
├── macos/              # macOS-specific configs
│   └── LaunchAgents/   # Launch agents
├── linux/              # Linux-specific configs
│   └── systemd/        # Systemd services
├── docker/             # Docker compose files
│   └── dev-services.yml
└── env/                # Environment configuration
    └── env.example
```

## 🚀 macOS Launch Agents

Place `.plist` files in:
- User agents: `~/Library/LaunchAgents/`
- Global agents: `/Library/LaunchAgents/`
- System daemons: `/Library/LaunchDaemons/`

### Example Usage

```bash
# Load a launch agent
launchctl load ~/Library/LaunchAgents/com.example.agent.plist

# Unload a launch agent
launchctl unload ~/Library/LaunchAgents/com.example.agent.plist
```

## 🐧 Linux Systemd

Place `.service` files in:
- User services: `~/.config/systemd/user/`
- System services: `/etc/systemd/system/`

### Example Usage

```bash
# Enable and start a service
systemctl --user enable my-service.service
systemctl --user start my-service.service

# Check service status
systemctl --user status my-service.service
```

## ⏰ Cron Jobs

Edit crontab:
```bash
crontab -e
```

Or store cron configurations as files for version control.

## 🐳 Docker Compose

Example for development services:
```yaml
version: '3.8'
services:
  postgres:
    image: postgres:latest
    restart: always
    environment:
      POSTGRES_PASSWORD: devpassword
    ports:
      - "5432:5432"
```

### Usage

```bash
# Start services
docker-compose -f docker/dev-services.yml up -d

# Stop services
docker-compose -f docker/dev-services.yml down
```

## ⚠️ Important

- Test startup configurations before adding to system
- Document any dependencies or prerequisites
- Use absolute paths in configuration files
- Never commit sensitive credentials
- Back up system before modifying startup configs
