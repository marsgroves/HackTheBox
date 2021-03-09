# HackTheBox
Hack The Box pen testing and challenges from https://hackthebox.eu

Here we have walkthroughs of Hack The Box.

<a href="https://www.youtube.com/watch?v=1t8Mt8wVgiY&t=152s">Hack The Box - Getting Started!</a>

In this demo, I will show you how to get started with hacking using Hack The Box! 
I'll give you a walkthrough and how you can get your "invite code" to get started. :)

        What Is Hack The Box?
It is an online platform that consists of virtual machines, and allows you to ethically test and advance your skills in penetration testing and cybersecurity. It contains a multifarious amount of challenges as well as various levels of machines of your choice that you can selectively hack (easy, medium, hard). Some of the challenges consists of real world simulation scenarios. Other challenges lean more toward a capture-the-flag (CTF) style of challenges. Hack The Box is especially recommended as an online platform of us if you have an interest in network security or information security.

        Getting Started
1. Visit the Hack the Box site at https://www.hackthebox.eu/
2. Read through its FAQs and check out the other tabs on there to explore what it has to offer if you'd like.
3. You will be told to go to https://www.hackthebox.eu/invite to join Hack The Box (HTB).
4. When you go the invite page, you will see a text box asking you for an <b>invite code</b>.
5. Right click on the page, and open <b>inspect element</b>. Alternatively, press Ctrl+Shift+I to open the Chrome Developers Tools.
6. Go through the elements tab and find a script with source (src) as: <b>/js/inviteapi.min.js</b>
7. So now, go to https://www.hackthebox.eu/js/inviteapi.min.js You will see a JS file titled <b>inviteapi.mini.js</b>

<a href="https://miro.medium.com/max/1864/1*pmXbnn4EjGZRKtJTKyYGEA.png">See the makeInviteCode which is highlighted
</a>

8. makeInviteCode looks interesting. So let’s go back to https://www.hackthebox.eu/invite and try to find its contents.
9. Next, go to the console tab in Chrome Developer Tools, and type <b>makeInviteCode()</b> and press ENTER. You will get a 200 Success status and data as shown below.

<a href="https://miro.medium.com/max/700/1*aMf_Gn0CLJNpRHVMz5zW5A.jpeg">See the hint and data</a>