---
icon: lucide/laptop-minimal-check
---
# :lucide-laptop-minimal: My "setup" 

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
