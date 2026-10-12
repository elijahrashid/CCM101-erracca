
# Firewall Configuration

## 1. Allow SSH Access

Command used:

    sudo ufw allow ssh

This command allows SSH connections on port 22 so administrators can remotely manage the server.

## 2. Configure the Default Deny Policy

Commands used:

    sudo ufw default deny incoming
    sudo ufw default allow outgoing

The first command blocks incoming connections unless they are explicitly allowed. The second command allows outgoing connections from the server.

## 3. Enable the Firewall

Command used:

    sudo ufw enable

This command activates the UFW firewall and applies the configured rules.

## 4. Allow Port 8080

Command used:

    sudo ufw allow 8080/tcp

This command allows incoming TCP traffic on port 8080 so users can access the web application.

## 5. Verify Firewall Rules

Commands used:

    sudo ufw status verbose
    sudo ufw status numbered

These commands display the firewall status, default policies, and configured rules.

## 6. Security Warning

If the firewall is enabled before allowing SSH, remote administrators may lose access to the server because incoming SSH connections could be blocked.

