**Before uploading your files**  
0. Check all "TODO" comments and for each, resolve it/raise an issue about it and then remove it's comment.  
1. ESLint all the JS files (Cut `editor.min.js` to desktop; open `cmd` in `/js/` folder; type `eslint *.js`; when finished, cut the `editor.min.js` back into the folder)/W3Clint all HTML/CSS files.  
2. Update the version number in options.html and manifest to the latest version number.  
3. Remove/comment `console.log`s/`console.dir`s from all JS files. <s>Run Replace function to remove all tab chars at the end of lines - `\t+$` Can cause problems like [this one](https://github.com/GaurangTandon/ProKeys/commit/3ece14b5aa09c08cd283a1cc1d736ceb178fa3f3)</s>  
4. Update the change log in options.html as well as on [github](https://github.com/GaurangTandon/ProKeys/edit/master/change_log.md)  
5. Make sure that the update fixes all the bugs listed for its milestone number.  
6. Check for an [update](http://quilljs.com/docs/download/) to quill version, and replace the "min.js" and "snow.css" files in our codebase.  
7. Minify all the files **except editor.min.js** (cut-paste it separately - it is a >200KB file, takes a _lot of time_ to minify).   
8. Copy all `imgs` from `Uncompressed` to `Compressed` in case they were updated.  
9. [**Testing**](https://github.com/GaurangTandon/ProKeys/blob/master/HOW_TO_TESTING.md)

**After updating the extension**  
0. Make sure to reply to all people on the [support page](https://chrome.google.com/webstore/detail/prokeys/ekfnbpgmmeahnnlpjibofkobpdkifapn/support) as well as on the official email (prokeys.feedback@gmail.com), whose errors have been fixed in this updated version.  
1. Update new cards (put them in their respective columns) on the [main project](https://github.com/GaurangTandon/ProKeys/projects/1) for the new issues that were filed while the development. This helps have laser sharp focus for the next update. (Also delete the column that was being used for this update.)  
2. Upload the compressed zipped file under [Releases](https://github.com/GaurangTandon/ProKeys/releases) and <s>the uncompressed files to master branch of codebase.</s> useless if I keep committing code frequently enough  
3. Update the [known bugs list](https://docs.google.com/document/d/1_MHKm1jtpJCWgksfbUdufExRFlF81S-IuTz1Czu7gOI/edit)  
4. Clone the previous folder of the files on the local dev pc and rename the new folder as `v_nxt_v_num`

**Please follow the following conventions:**

1. All class names in HTML must be in small case. Multiple words should be separated by underscore.
2. Snippet parts should be referred to as "name" and "body" respectively.
3. All variables names related to a HTML Node should EITHER have $ at the start of their name OR contain the word "node" (not elm) in their name.
