<div align="center">

## How to send an email in ASP\.net


</div>

### Description

Sending email in ASP.NET is a breeze! Check out this example. Note that docs say that the .SMTPServer property is optional...if you don't specify one, Windows queues up your email for you. However, I haven't tested out this method of sending mail.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Ian Ippolito \(vWorker\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/ian-ippolito-vworker.md)
**Level**          |Beginner
**User Rating**    |4.3 (47 globes from 11 users)
**Compatibility**  |VB\.NET, ASP\.NET
**Category**       |[Internet/ Browsers/ HTML](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/internet-browsers-html__10-9.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/ian-ippolito-vworker-how-to-send-an-email-in-asp-net__10-161/archive/master.zip)





### Source Code

```
Dim mmMail As New System.Web.Mail.MailMessage()
  Dim objSmtpServer As System.Web.Mail.SmtpMail
  mmMail.From = "me@me.com"
  mmMail.To = "you@you.com"
  mmMail.Subject = "My subject"
  mmMail.Body = "My body"
  objSmtpServer.SmtpServer = "my smtp server"
  objSmtpServer.Send(mmMail)
```

