# AppCloud updates July 2011

The updates described are either important (where you need to take action) or of interest (you might want to know about these changes but you don't need to do anything). 


---

<a href=#update4><h2 id="update4"> **Action Req'd:** Upgrade to Ruby 1.8.7-p352 </h2></a>

July 22nd, 2011 (scheduled)

AppCloud will be upgraded to Ruby 1.8.7-p352 on or around July 22nd. 

If you are using Ruby 1.8.7 and Unicorn, you must redeploy after updating.

If you are using Ruby 1.8.7 and Passenger, we recommend that you redeploy after updating. This is to make sure that your code runs under the latest version of the MRI interpreter.


---

<a href=#update3><h2 id="update3"> Minor: Increased maximum connections for HAProxy </h2></a>

July 8th, 2011

The maximum number of connections for HAProxy increased to 65,535 from 15,000.

---

<a href=#update2><h2 id="update2"> Minor: Upgrade to Redis 2.2.11</h2></a>

July 8th, 2011

For more information, see the [[Redis 2.2 release notes|https://github.com/antirez/redis/blob/2.2.11/00-RELEASENOTES]].

---

<a href=#update1> <h2 id="update1"> Minor: Nginx Upload Progress module upgraded </h2></a>

July 1st, 2011

The nginx_uploadprogress_module was upgraded to address a vulnerability in certain configurations. 

For information, see [[nginx package in Lucid Lynx allows null byte vulnerability|https://bugs.launchpad.net/ubuntu/+source/nginx/+bug/783508]].



[1]: #update1        "update1"
[2]: #update2        "update2"
[3]: #update3        "update3"
[4]: #update4        "update4"
[5]: #update5        "update5"
[6]: #update6        "update6"
[7]: #update7        "update7"
[8]: #update8        "update8"
[9]: #update9        "update9"
[10]: #update10        "update10"
[11]: #update11        "update11"
[12]: #update12        "update12"
[13]: #update13        "update13"
[14]: #update14        "update14"