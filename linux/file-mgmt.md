Linux file mgmt cheats
======================

<h4>File Commands</h4>
<pre>
diff file1 file 2    #compare two files
md5sum -t file    #compute hash
echo -n “string” | md5sum    #generate hash of string
sha1sum   #sha1 hash of file
find / -name string   #find string or file name
find -i -name file-name -type *.pdf   #find files of pdf type
</pre>

<h4>Package Commands:</h4>
<pre>
tar cf file.tar files    #create tar package
tar czf file.tar.gz files  #creates tar.gz package
tar cjf file.tar.bz2 files   #creates .bz2 package
tar xf file.tar    #extract
tar xzf file.tar.gz    #extract
tar xjf file.tar.bz2    #extract
zip -r filename.zip directory    #creates zip archive of the directory and sub directories
 </pre>


<h4>dd Commands</h4>
<pre>
dd skip =1000 count=2000 bs=8 if=file of=file   #cut blocks 1000 to 3000 from file
dd if=/dev/urandom of=<file> bs=3145728    #create random 3mb file
</pre>

<h4>Ownership</h4>
<pre>
$ sudo chown -R hduser:hadoop /usr/local/hadoop  #recursive ownership 
</pre>