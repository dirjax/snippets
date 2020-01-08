# snippets


```for files in $(find . -mindepth 1 -type f -not -iname ".gz") ; do if [[ "$(lsof ${files} ; echo $?)" == "1" ]] ; then gzip ${files}; else echo "keeping ${files}"; fi; done```
