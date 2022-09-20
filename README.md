# No ad youtube
<p style="text-align:center">
<img width="50%" src="doc/demo.gif"/>
</p>
This project is a proof of concept, it explores the use of youtube's embed architecture to circumvent ads

## Quickstart
```
npm install
node .
```

## Also Ngrok
Forward this service to the web using ngrok, and avoid being canceled by youtube 
1. [Make an ngrok account](https://ngrok.com/)
2. Create an ssh key with the command `ssh-keygen`
   1. Follow the prompts, remember the passphrase 
   2. Copy the public key (cat /path/to/key.pub)
3. [Paste the ssh key to ngrok](https://dashboard.ngrok.com/tunnels/ssh-keys)
4. Forward the webite to the web
```bash
ssh -i id_rsa -R 443:localhost:<PORT> tunnel.us.ngrok.com http
```
The output should be two routes, one with ssl enabled