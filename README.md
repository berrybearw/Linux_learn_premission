# Linux_learn_premission
Linux 權限

# Linux 權限

參考 : [https://superuser.com/questions/648163/recursively-chown-all-files-that-are-owned-by-a-specific-user](https://superuser.com/questions/648163/recursively-chown-all-files-that-are-owned-by-a-specific-user)

改檔案修改權 

chmod 

改檔案用戶與群組

chown

大量調整檔案

`find . -type d -iname '???' -user old_user -exec chown -R new_user:new_group {} \;`

測試情境

`find . -type d -iname 'zh_TW' -user tiptop -exec chown -R tiptop:tiptop {} \;`

> 找出目錄名稱為 zh_TW 用戶為 tiptop 執行更改此目錄全部檔案
> 
> 
> 用戶 tiptop 群組 tiptop
>
