# Simple-Bash-Scripts
A collection of bash scripts.
<div class="entry-head ">
<h1 class="entry-title">How to run .sh or Shell Script file in Windows 10</h1>
<span id="ezoic-pub-ad-placeholder-894"></span>
<div class="entry-submeta">&nbsp;</div>
</div>
<div class="row">
<div class="col-md-8 col-sm-12 col-xs-12">
<div class="y-link-underline">
<div class="entry-affiliate" align="center"><strong><a href="http://www.restoro.com/includes/route.php?tracking=twc&amp;lpx=lwdu" rel="nofollow">Download this PC Repair Tool to quickly find &amp; fix Windows errors automatically</a></strong></div>
<div class="entry-content">
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="4">&nbsp;</div>
<p><strong>Shell Scripts</strong>&nbsp;or<strong>&nbsp;.SH files</strong>&nbsp;are like batch files of Windows which can be executed in Linux or Unix. It is possible to run .sh or Shell Script file in Windows 10 using Windows Subsystem for Linux. In this post, we will show you how to run a Shell Script file in Windows 10.<span id="ezoic-pub-ad-placeholder-679" class="ezoic-adpicker-ad"></span></p>
<h2>How to run .sh or Shell Script file in Windows 10</h2>
<p><strong>Bash</strong>&nbsp;is a&nbsp;Unix shell&nbsp;and&nbsp;command language which can run Shell Script files. You do not need to install Ubuntu or any other Linux Distros unless your scripts need the support of the real Linux kernel. We will share both the methods.</p>
<ol>
<li>Execute Shell Script file using WSL</li>
<li>Execute Shell Script using Ubuntu on Windows 10</li>
</ol>
<h3>1] Execute Shell Script file using WSL</h3>
<p><strong>Install WSL or Windows Subsystem for Linux</strong></p>
<div class="code-block code-block-16">&nbsp;</div>
<p>Go to&nbsp;Settings &gt; Update &amp; Security &gt; For Developers. Check the&nbsp;<em>Developer Mode</em>&nbsp;radio button. And search for &ldquo;<em>Windows Features</em>&rdquo;, choose &ldquo;<a href="https://www.thewindowsclub.com/ways-to-enable-or-disable-optional-windows-features"><em>Turn Windows features on or off</em></a>&rdquo;.</p>
<div class="code-block code-block-1">&nbsp;</div>
<p>Scroll to find WSL, check the box, and&nbsp;<a href="https://www.thewindowsclub.com/run-bash-on-windows-10">then install it</a>. Once done, one has to reboot to finish installing the requested changes. Press Restart now.&nbsp; BASH will be available in the Command Prompt and PowerShell.</p>
<div class="code-block code-block-2"><span id="ezoic-pub-ad-placeholder-144"></span>
<div id="google_ads_iframe_/1254144/thewindowsclub_com-box-3_0__container__"><iframe id="google_ads_iframe_/1254144/thewindowsclub_com-box-3_0" title="3rd party ad content" src="https://e841addd593742f319b0a999b1b345ca.safeframe.googlesyndication.com/safeframe/1-0-37/html/container.html" name="" width="300" height="250" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" sandbox="allow-forms allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-top-navigation-by-user-activation" data-is-safeframe="true" data-google-container-id="w" data-load-complete="true"></iframe></div>
</div>
<p><strong>Execute Shell Script Files</strong></p>
<ol>
<li>Open Command Prompt and navigate to the folder where the script file is available.</li>
<li>Type Bash script-filename.sh and hit the enter key.</li>
<li>It will execute the script, and depending on the file, you should see an output.</li>
</ol>
<p><img class="aligncenter size-large wp-image-186225 lazy-loaded" src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-600x295.png" sizes="(max-width: 600px) 100vw, 600px" srcset="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt.png 600w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-150x74.png 150w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-400x197.png 400w" alt="Run Shell script files from Command Prompt" width="600" height="295" data-lazy-type="image" data-src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Shell-script-files-from-Command-Prompt-600x295.png" data-srcset="" /></p>
<p>On a Linux platform, you usually use SH, but here you need to use BASH. That said, BASH in Windows has its limitations, so if you want to execute in a Linux environment, you need to install Ubuntu or anything similar.</p>
<div class="code-block code-block-3"><span id="ezoic-pub-ad-placeholder-153"></span>
<div id="google_ads_iframe_/1254144/thewindowsclub_com-medrectangle-3_0__container__"><iframe id="google_ads_iframe_/1254144/thewindowsclub_com-medrectangle-3_0" title="3rd party ad content" src="https://e841addd593742f319b0a999b1b345ca.safeframe.googlesyndication.com/safeframe/1-0-37/html/container.html" name="" width="580" height="400" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" sandbox="allow-forms allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts allow-top-navigation-by-user-activation" data-is-safeframe="true" data-google-container-id="l" data-load-complete="true"></iframe></div>
</div>
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="1">&nbsp;</div>
<p><iframe class="lazy-loaded" title="How to run  sh or Shell Script file in Windows 10" src="https://www.youtube.com/embed/06E5etw4sqk?feature=oembed" width="750" height="422" frameborder="0" allowfullscreen="allowfullscreen" data-lazy-type="iframe" data-src="https://www.youtube.com/embed/06E5etw4sqk?feature=oembed"></iframe></p>
<div class="code-block code-block-4">&nbsp;</div>
<h3>2] Execute Shell Script using Ubuntu on Windows 10</h3>
<p>Make sure you have&nbsp;<a href="https://www.thewindowsclub.com/run-bash-on-windows-10">Ubuntu or any other Linux distros installed</a>.&nbsp; Ubuntu will mount or make all your Windows directories available under&nbsp;<em>/mnt</em>. So the C drive is available at&nbsp;<em>/mnt/C</em>.&nbsp; So if the desktop will be available at&nbsp;<em>/mnt/c/users/&lt;username&gt;/desktop</em>.</p>
<p><img class="aligncenter size-large wp-image-186224 lazy-loaded" src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-600x187.png" sizes="(max-width: 600px) 100vw, 600px" srcset="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu.png 600w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-150x47.png 150w, https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-400x125.png 400w" alt="Run Script files in Windows via Ubuntu" width="600" height="187" data-lazy-type="image" data-src="https://www.thewindowsclub.com/wp-content/uploads/2019/07/Run-Script-files-in-Windows-via-Ubuntu-600x187.png" data-srcset="" /></p>
<p>Now follow these steps</p>
<ol>
<li>Type Bash in run prompt, and it will launch the distro prompt.</li>
<li>Navigate to the folder using &ldquo;cd&rdquo; command to the folder where the scripts are available.</li>
<li>Type &ldquo;sh script.sh&rdquo; and hit enter.</li>
</ol>
<p>It will execute the script, and if they have a dependency on any of core Linux features.</p>
<div class="code-block code-block-5">&nbsp;</div>
<div class="c24ff8f4a2da697123def04f69833d8b" data-index="3"><strong><a href="http://www.restoro.com/includes/route.php?tracking=twc&amp;exec=run" rel="nofollow noopener">Download PC Repair Tool to quickly find &amp; fix Windows errors automatically</a></strong></div>
<p>Since Linux is now available in Windows, you need not use any third party applications like Cygwin. WSL should be enough for most of the scenarios to help you run a shell script in Windows 10.</p>
<div class="code-block code-block-6">&nbsp;</div>
</div>
</div>
</div>
</div>
