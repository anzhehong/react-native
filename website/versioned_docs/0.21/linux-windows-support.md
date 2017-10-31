---
id: version-0.21-linux-windows-support
title: linux-windows-support
original_id: linux-windows-support
---
<a id="content"></a><table width="100%"><tbody><tr><td><h1><a class="anchor" name="linux-and-windows-support"></a>Linux and Windows Support <a class="hash-link" href="undefined#linux-and-windows-support">#</a></h1></td><td style="text-align:right;"><a target="_blank" href="https://github.com/facebook/react-native/blob/master/docs/LinuxWindowsSupport.md">Edit on GitHub</a></td></tr></tbody></table><div><p><strong>NOTE: This guide focuses on Android development. You'll need a Mac to build iOS apps.</strong></p><p>As React Native on iOS requires a Mac and most of the engineers at Facebook and contributors use Macs, support for OS X is a top priority. However, we would like to support developers using Linux and Windows too. We believe we'll get the best Linux and Windows support from people using these operating systems on a daily basis. </p><p>Therefore, Linux and Windows support for the development environment is an ongoing community responsibility. This can mean filing issues and submitting PRs, and we'll help review and merge them. We are looking forward to your contributions and appreciate your patience.</p><p>As of <strong>version 0.14</strong> Android development with React native is mostly possible on Linux and Windows. You'll need to install <a href="https://nodejs.org/" target="_blank">Node.js</a> 4.0 or newer. On Linux we recommend installing <a href="https://facebook.github.io/watchman/docs/install.html" target="_blank">watchman</a>, otherwise you might hit a node file watching bug.</p><h2><a class="anchor" name="what-s-missing-on-windows"></a>What's missing on Windows <a class="hash-link" href="docs/linux-windows-support.html#what-s-missing-on-windows">#</a></h2><p>On Windows the packager won't be started automatically when you run <code>react-native run-android</code>. You can start it manually using:</p><div class="prism language-javascript">cd MyAwesomeApp
react<span class="token operator">-</span>native start</div><p>If you hit a <code>ERROR  Watcher took too long to load</code> on Windows, try increasing the timeout in <a href="https://github.com/facebook/react-native/blob/master/packager/react-packager/src/DependencyResolver/FileWatcher/index.js#L16" target="_blank">this file</a> (under your node_modules/react-native).</p></div><div class="docs-prevnext"><a class="docs-next" href="tutorial.html#content">Next →</a></div>