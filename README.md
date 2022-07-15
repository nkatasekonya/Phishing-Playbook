## Playbook: Smishing   
Smishing is a phishing attack carried out via the Short Message Service (SMS). Threat actors send users text messages purporting to be from a reputable 
company with the intent of tricking user to reveal personal information such as their identification number (which can lead to identity theft) or 
passwords. In the more extreme situations redirecting users to sites that contain  malicious software.  
![Smishing Example](https://i0.wp.com/dufeu-it.co.uk/wp-content/uploads/2021/09/smishing-blog-header.jpg)

**Disclaimer**  
*- This playbook is intended for educational purposes and may not necessarily represent the state-of-the-art, as such it might be updated from time to time. The goal is to introduce students/beginners to incident response. Feel free to contribute content relevent to the topic*  
*- It is adviced that investigations be carried out in an isolated enviroment such as a VM to avoid accidentally infecting your machine*

### Investigating Smishing
1. **URLs**
   - URLs in messages are shown “as-is”, making it reletively easy to spot suspicious one. The URL should be compared to that of the company the threat actors are claiming to represent. Threat actors will usually add a hyphen, or an extra letter in the domain to trick users into thinking that it is the original domain.
   - To conceal malicious URLs the attackers often use URL shorteners or in some cases send you to an actual site which then redirects you to a malicious one
   - Suspicious URLs should not be opened as they may send users to sites that contain malicious software, they should only be opened in isolated enviroments to monitor their impact, (more on this later).
1. **Convert short URLs to “expanded” URLs**
   - Because it can be difficult to determine the validity of a URL when it has been shortened, the URL should be *"expanded"*
   - [expandurl.net](https://www.expandurl.net/) is a service where you can find an expanded version of a shortened URL and other metadata about the destination site
3. **Open URLs using free online service**
   - While you can setup an enviroment in a VM to investigate the impact of running a suspected URL, in this guide we focus on accessible online services
   - 
5.
6.
7.

**Additional Information**
1. [Learn How to Forensically Examine Phishing Emails to Better Protect Your Organization Today](https://www.knowbe4.com/hubfs/KB4-ForensicsPhishing_Slides.pdf?hsLang=en)
1. [incident-response-plan-template](https://github.com/counteractive/incident-response-plan-template)

`TODO: add an example analysing a smishing attack`  
`TODO: model around Investigate, Remediate (contain, eradicate), and Communicate`
