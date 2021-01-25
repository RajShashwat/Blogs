## Resolving Ubuntu Boot-Time Freezing Issue(for Systems having Nvidia Graphics)

As * **NVIDIA** has low compatibility with **Linux ** *so it causes the problem of **freezing** when drivers are not installed properly. When we install a Linux in a system having Nvidia Graphics the system freezes causing the unnecessary problem to the user. Event some times it interferes with other drivers and causing problem liking heating of laptop fan not working etc.

In this article, I will discuss how to avoid freezing when booting Ubuntu in systems having Nvidia Graphics.

A few days ago, I decided to switch from Windows to Ubuntu and the same problem happened with me. While installing Ubuntu my system froze and was not responding and I had to shut it down forcefully.

I have HP Pavilion Gaming Laptop which comes with NVIDIA GeForce GTX 1050 and has *Windows 10* pre-installed on the 128 GB SSD and 1 TB of HDD. When I removed windows and installed Ubuntu. It was showing the purple screen then it froze there. Nither mouse nor keyboard was working. I had to turn off the device by holding the power button. And it was the same story every time I started my laptop.


![purple screen.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1611567832501/sKkZPgSys.png  "Purple Ubuntu Screen Freeze")

I had to work for two continuous days trying to find out what the problem was I installed different versions of Ubuntu and took my laptop to HP Service centre to check if there was a problem with my laptops Hardware. **Finally, I found the problem lied with Graphis compatibility.**

If you have a similar problem this is how you can solve it.

Let’s see how to avoid/overcome this problem.

There are many temporary solutions to this but I will discuss the most optimal and permanent way of avoiding this issue.

## Step 1:

**While installing Ubuntu, make sure to disable your graphics.**

While installing you will be directed to the Grub menu, there you will see different options. You have to continue with the option of “safe graphic”. Safe Graphics Option is available in ubuntu 19.04 & above. If you go for “normal installation” there are chances that your system will freeze even while installing Ubuntu.

So to avoid this go with the “safe graphic” option.


![safegraphics.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568068211/tbV2Vluny.png "Select Install Ubuntu (safe Graphics)")

## Step 2:

While installing connect your system to the internet and select the option *Download updates while installing Ubuntu.*

This will ensure your system downloads a driver for Nvidia Graphics.

Skipping this option may again lead to freezing of your system while booting into it.


![download.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568177972/hECu2Xzg2.png "Check the Download Updates while installing Ubuntu
" )

Step 3:
When you successfully install Ubuntu and restart your system. Open the Additional Driver from the menu and wait for a few seconds.


![Screenshot from 2020-12-25 17-27-16.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568221136/e8UKgyfTZ.png "Click on Additional Driver" )

It will show all the proprietary drivers available. Select any proprietary driver and click apply the change.


![Screenshot from 2020-12-25 17-25-01.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568270959/EAzqDONAr.png " Select any Proprietary Driver " )

It will install the new driver.


## Step 4:

If you have a UEFI secure boot(as in my case) enabled, it will ask you to set a password (you can set any simple password). Enter Your Password And press Next.


![Screenshot from 2020-12-25 17-35-45.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568376206/rwys-GAa3.png)

Once the installation finishes, it will ask you to restart the system.

## Step 5:

Once you restart your system you will see a purple screen with options. You can either choose:

-**Continue boot**
or
-**Enroll MOK**

With Continue boot there are chances that all the features of the new driver won’t work correctly.

That’s why you should go with **Enroll MOK**

Select Enroll MOK and press Enter

![mok0.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568737860/SQxM7JGVm.jpeg)

Then you will move to the next page saying [Enroll MOK]. Select Continue and press Enter.


![mok2.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568771924/OO3b79RzK.jpeg)

This will again lead you to a new page asking you to Enroll the key? Select Yes and press ENTER


![mok3.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568793577/Ngq412BFZ.jpeg)

This will again lead you to a new page asking you to Enroll the key? Select Yes and press ENTER


![mok4.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568803683/LUMKHNcU9.jpeg)

It just shows this screen, You enter your password here and press Enter.
Then at last it will ask to reboot your system. Select Reboot and press Enter.


![mok5.jpg](https://cdn.hashnode.com/res/hashnode/image/upload/v1611568831010/01jnU6Ig_.jpeg)

This will restart your system.

This will solve your problem of freezing which happens due to the incompatibility of Nvidia with Linux.