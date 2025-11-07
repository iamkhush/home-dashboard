# Home Dashboard

The **Home Dashboard** is a web-based dashboard designed to be displayed on a tablet for use in a household.

## Project Structure

- `index.html`: The main HTML file for the dashboard.
- `devops/`: Contains Nginx configuration templates and deployment scripts.

## Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd home-dashboard
   ```

2. **Configure Nginx**
   - Use the provided Nginx configuration templates in `devops/` to set up the server.
   - Ensure the `location.conf.j2` template is correctly configured for your environment.

3. **Deploy the Dashboard**
   - Use the provided Ansible playbook to deploy the dashboard:
     ```bash
     ansible-playbook devops/ansible-playbook.yml
     ```

4. **Access the Dashboard**
   - Open a browser and navigate to the configured domain (e.g., `https://chaddas.home`).

## Requirements

- Nginx
- Ansible
- A web server with access to `/var/www/html`

