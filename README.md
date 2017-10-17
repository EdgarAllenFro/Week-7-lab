# Project 7 - WordPress Pentesting

Time spent: **11-12** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) Brute Force Password
  - [ ] Summary: Brute force of password using WpScan built in brute forcer tool
    - Vulnerability types:dictionary attack
    - Tested in version: 4.2
    - Fixed in version:n.a
  - [ ] GIF Walkthrough:https://github.com/EdgarAllenFro/Week-7-lab/blob/master/Brute_force_wpscan.gif
  - [ ] Steps to recreate: In the command line, go to the location on the system where wpscan is located. Once there run the command 
  [ruby wpscan.rb --url(website) --wordlist(dictionary of passwords) --username(user to test)]
    - [Link 1](http://www.hackingtutorials.org/web-application-hacking/hack-a-wordpress-website-with-wpscan/)
1. (Required) DOM XSS attack on WP
  - [ ] Summary:Any wp theme or plugin that uses genericons is vulnerable to a DOM based XSS executed through the url 
    - Vulnerability types:XSS,Themes/plugins
    - Tested in version:4.2
    - Fixed in version: theme:twentyfifteen version 1.2
  - [ ] GIF Walkthrough:https://github.com/EdgarAllenFro/Week-7-lab/blob/master/XSS1_WP.gif
  - [ ] Steps to recreate: tag your xss to the end of a url bound to location [http:// site.com/wp-content/themes/twentyfifteen/genericons/example.html#1] 
  - [ ] Affected source code:genericons using themes or plugins
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:4.2
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

## Assets

In addition to wpscan and wpdistillery, i sed the wordlist from the cain and abel cracker to run the admin password against.

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)
- [WPScan Brute](http://www.hackingtutorials.org/web-application-hacking/hack-a-wordpress-website-with-wpscan/)
- [DOM XSS Genericons](https://blog.sucuri.net/2015/05/jetpack-and-twentyfifteen-vulnerable-to-dom-based-xss.html)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2017] [Ben Wiggins]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
