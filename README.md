# NTUT_HOMEWORK
# Exchange server
## 事件起源
臺灣資安業者戴夫寇爾（DEVCORE）是在去年12月發現ProxyLogon中的CVE-2021-26855與CVE-2021-27065兩個安全漏洞，並於今年1月5日通報微軟，另一資安業者Volexity則說駭客自1月3日便開始攻擊ProxyLogon漏洞，至於微軟則直接點名該駭客組織為來自中國的Hafnium。
## ProxyLogon為什麼這麼嚴重
Exchange Server上被建立web shell程式，這種程式可能被駭客當成後門，以便用來竊取郵件、或執行程式碼。
存取Exchange系統能讓他們取得重要憑證，用於日後其他攻擊。例如他們可能藉此取得網域管理員帳號，或是具備援權限的服務帳號。這樣一來，攻擊者就能Exchange事件之後許久，在網路環境下發動勒索軟體或竊密行動。
## ProxyLogon的攻擊本質?
駭客的攻擊路徑類似，在利用ProxyLogon漏洞進駐受駭者系統之後，會先植入惡意的Web Shell，再安裝額外的惡意程式。
