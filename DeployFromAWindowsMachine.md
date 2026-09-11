## First "Steam" beyond the fences - Email provider opensource
where `eldervibe.dev` is my personal domain can be replaced by yours

### Configurate DNS
1. On DNS server, add these records:
```
A      mail.eldervibe.dev      <YOUR_VPS_IP>

MX     eldervibe.dev           10 mail.eldervibe.dev
```
2. On dev machine run these commands to check domain resolver
```
nslookup -type=mx eldervibe.dev
nslookup mail.eldervibe.dev
nslookup <YOUR_VPS_IP>
```
3. Then on the vps trying to reverse DNS
At this step only people who owns the ip/vps can do, in my case it's Hostkey.
> PTR

-> I'm writing an email to the Hostkey team to enable it:
> Hello Hostkey Support Team,
I am setting up a self-hosted mail server on my VPS and would like to request a reverse DNS (PTR) record for my server IP.
IP Address: <YOUR_VPS_IP>
Desired PTR Hostname: mail.eldervibe.dev
The forward DNS has already been configured as follows:
mail.eldervibe.dev -> <YOUR_VPS_IP>
Could you please configure the corresponding reverse DNS entry:
<YOUR_VPS_IP> -> mail.eldervibe.dev
Please let me know if any additional verification or information is required.
Thank you for your assistance.
Best regards,