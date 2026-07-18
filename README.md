# Remote Desktop Connection via GitHub Actions

This repository uses GitHub Actions to automatically create a remote desktop connection via Ngrok, allowing secure access to a Windows environment. Each GitHub Action execution generates an Ngrok tunnel that lasts for approximately 1 hour, enabling RDP (Remote Desktop Protocol) access.

### Key Features:
- **Automated Setup**: Uses GitHub Actions to set up and configure a remote desktop session.
- **Secure Tunnel**: Ngrok provides a secure tunnel for RDP access.
- **Quick Access**: Each session lasts about 1 hour, with easy reconnection using the IP provided by Ngrok.

<h2 align="left">👤 Repo Visitors:</h2>
<p align="left">
<a href="https://rojansapkota.com.np" target="_blank">
<img src="https://profile-counter.deno.dev/RojanSapkota_Remote-Desktop-Connection/count.svg" alt="Visitor Counter"/>
</a>
</p>

### Installation & Setup:
1. Fork the repository.
2. Replace the `NGROK_AUTH_TOKEN` in the GitHub Actions workflow file with your Ngrok authentication token.
3. Set the `NGROK_AUTH_TOKEN` in GitHub by adding it as an environment variable in your repository’s secrets.
   - Go to **Settings > Secrets > Actions** in your GitHub repo and add a new secret named `NGROK_AUTH_TOKEN`.
4. Trigger the GitHub Action by pushing any change or using the **workflow_dispatch** event.
5. Once the action runs successfully, Ngrok will provide an IP address and port.
6. Use Remote Desktop Connection to connect to the provided IP and port.

### Contributing:
Feel free to submit pull requests or open issues for improvements or bug fixes.
