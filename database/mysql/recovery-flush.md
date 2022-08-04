# Recovery/Flush

InnoDB uses a background thread to periodically flush the changes to the data file.



![](<../../.gitbook/assets/스크린샷 2022-07-29 오후 5.40.59.png>)



The Overall log file is controlled by _innodb\_log\_files\_in\_group . The total size is the sum of each file's size._&#x20;





![](<../../.gitbook/assets/스크린샷 2022-07-29 오후 5.38.44.png>)

