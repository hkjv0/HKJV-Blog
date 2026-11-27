---
icon: lucide/laptop-minimal-check
---
# :lucide-laptop-minimal: My "setup" 
   27/nov/26
!!! note "Read this first"
    This is my personal experience, not a recommendation for everyone.
    What works for me depends on my threat model and my tolerance for friction.

## :simple-grapheneos: Graphene OS - Pixel 7

Graphene OS, the most secure and private mobile operating system you can get. I started using Graphene in mid-2025 with a used Pixel 7 that I bought specifically to run this OS. I’ve been using it as my primary phone ever since and have grown quite attached to it, even though I plan to get a Pixel 8+ (and if you’re thinking of using Graphene OS, I recommend you do the same), since the Pixel 7 lacks MTE and its update support is “almost” over.

**Interesting features that GOS has that other AOSP-based operating systems don't:**

   -[:simple-googleplay:]**Sandboxed & Optional Play Services:** One of the first things I liked about GOS is that it lets you choose whether or not to use Google’s services and its store, and if you need or want to use them, they install just like any other app that is, without elevated privileges. 

!!! tip 
    Unless your threat model calls for it, I recommend using the Google Play Store-it’s one of the most secure app stores you can use. Someday I’ll talk about why not everything from Google is actually bad.

   -[:lucide-shredder:]**Duress PIN/Password:** This is a very interesting feature (and if you're interested in these topics, you've probably already heard some news about it) that lets you set a PIN or passcode; when you enter it, your phone irreversibly deletes all your data, which in certain situations can be a crucial last resort.

   -[:simple-googlechrome:]**Vanadium:** Does it really need an introduction? The best description of this browser is the one provided by the project itself: "Vanadium is a hardened variant of Chromium providing enhanced privacy and security, similar to how GrapheneOS compares to AOSP.", in my opinion (and that of many others) this browser is the best you can get.

**Downsides of Graphene OS in Daily Use**

   -[:lucide-landmark:]**Online Banking Apps:** Usually, when someone online recommends Graphene OS, the first concern or question is whether banking apps are compatible. This hasn’t been an issue for me, since my banks are fully compatible with Graphene OS. It’s important to note that if your banking app isn’t compatible with Graphene OS, it’s **not** the project’s fault it’s because the bank or similar entity has explicitly blocked it, For example, the only app I can’t use is my brokerage app; however, after sending them an email, they told me it wasn’t intentional and they’re already fixing it (at least now I can use it on the web without any problems).

## :simple-qubesos: Qubes OS - Thinkpad T480s

Qubes OS is an operating system whose entire architecture is based on the principle of security through compartmentalization, using VMs called Qubes. There are typically two types of VMs: templates and AppsVMs. AppsVMs are based on a template; however, an AppsVM cannot write to the template, while the template can write to the AppsVM, This ensures that if an AppVM is compromised, it cannot compromise other AppVMs using the same template. I currently use Qubes OS as my daily driver on a T480s, which I plan to replace in a few months with a model that still receives firmware updates. However, the reason I chose it is because it works out of the box with Qubes.

**Interesting Features and Implementations of Qubes OS**

   -[:lucide-hard-drive:]**Ultra-lightweight templates and AppVMs:** Unlike VirtualBox, where cloning a machine duplicates the entire system, Qubes separates the software from your data. Multiple VMs share the same read-only template, so having ten isolated environments takes up barely as much disk space as your personal files. Although many Type 2 hypervisors DO allow something similar, it’s not as easy to achieve; in Qubes, however, it’s available right out of the box.
   
   -[:lucide-shield-check:]**Global clipboard with isolation:** Each virtual machine has its own isolated clipboard so that no malware can spy on what you copy. To transfer text between them, you must use a specific key combination (Ctrl + Shift + C/V) that clears the global buffer immediately after use.

**Disadvantages and Limitations of Qubes OS**

   -[:lucide-book-search:]**Steep learning curve and limited support:** If something goes wrong in VirtualBox, you can fix it using a user-friendly graphical interface or by reinstalling the program. In Qubes OS, troubleshooting network errors, USB device issues, or failed updates usually requires solid knowledge of the Linux terminal and an understanding of its internal permission architecture. Personally, even though I’ve been using Qubes for almost a year now, I still consider myself a beginner.

## :lucide-lock-keyhole: Secureblue - Dell Inspiron 3515

Secureblue is a security-focused Linux operating system for desktops and servers. Secureblue’s goal is to maximize the security that Linux can offer desktop and server users; since Linux lacks many security features and implementations, Secureblue aims to at least mitigate some of the security vulnerabilities that a Linux user might face. Personally, I see Secureblue as a little brother to Graphene OS; although it doesn’t offer the same level of security as its “big brother,” compared to other Linux-based desktop operating systems, Secureblue truly makes an effort to improve security. As they say: Secureblue is recommended for people who want Linux first and security second.

**Interesting features of Secureblue that other Linux desktop operating systems don't have—or that most don't have:**

   -[:simple-googlechrome:] **Trivalent:** Like Graphene OS, Secureblue has its own browser, which as I mentioned in my post about Graphene OS is one of the best browsers you can use if you're on a Linux desktop; it's inspired by Vanadium.

   -[:lucide-shield-check:] **Security by default and out-of-the-box hardening:** Personally, this is what I like most about Secureblue: compared to most Linux-based operating systems, Secureblue lets you perform additional hardening (on top of what it ALREADY INCLUDES) without having to spend time researching and testing all it takes is a single command.


