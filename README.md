This project has been copied over from http://code.google.com/p/logkext on 15 January 2013


 <h1><a name="Introduction"></a>Introduction<a href="#Introduction" class="section_anchor"></a></h1><p><strong>logKext v2.3</strong> </p><p>Release Date: 2009-11-18 </p><p>Summary: LogKext is an open source keylogger for Mac OS X, a product of FSB software. </p><p>Requirements: Mac OS X 10.5 or 10.6 </p><h1><a name="Details"></a>Details<a href="#Details" class="section_anchor"></a></h1><p>How to get started: Control and usage of logKext is through logKextClient. LogKextClient runs through the Mac OS X Terminal.  </p><p>Step 1: Finding the Terminal </p><p>Locate the Terminal Application (/Applications/Utilities/Terminal) </p><p>Step 2: Using the Terminal </p><p>The window that pops up will have a command prompt that looks something like this:  [Bill&#x27;s-Computer:~] bill%  At the prompt type the following command and press return:  </p><p>sudo logKextClient </p><p>You will be prompted for your account password (you must be an administrator). Enter it. </p><p>Next, logKext will prompt you for your logKext password:  </p><p>logKext password: </p><p>Type in your logKext password. The default password is &quot;logKext&quot;. You will not see the password echoed to the screen as you type it.  </p><p>Step 3: Operating logKextClient </p><p>LogKextClient is an interactive client that allows you to change preference values that will change the behavior of your keylogger. Type &quot;help&quot; to get the help screen. </p><p>Most likely, you will want to see the logfile! To do this, use the &quot;open&quot; command. It will save the decrypted logfile to your desktop, and open it in a text editor. If you haven&#x27;t yet typed 100 characters, you will not yet have a logfile. Come back later and try again.  </p><p>Uninstalling logKextClient </p><p>A standalone script has been installed in your computer&#x27;s root directory that will uninstall logKext. It is called LogKextUninstall.command.  </p><p>Most Frequently Asked Question: Why is my logfile all gibberish? </p><p>If you have changed your password or turned encryption on or off, you must delete the logfile before these changes take effect; otherwise your client will try to decrypt using a different password than your daemon is encrypting: this results in &quot;gibberish.&quot; </p><p>Use the logKextClient &quot;list&quot; command to see where your logfile is, then quit logKextClient. Find the logfile using the path, and throw it in the trash. If you try to empty the trash, don&#x27;t worry if it says &quot;File is in use.&quot; After a while, you will be able to delete it. </p><p>You can also delete the logfile from the terminal if you know how (<tt> &quot;rm &lt;path&gt;&quot; </tt>) When asked to override permissions, type &quot;yes&quot;.  </p><p><strong>Note: For security reasons, it is recommended that you change your password from the default setting.</strong> </p>
