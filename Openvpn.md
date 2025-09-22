
DNS 못찾는 이슈

profile.ovpn 에 아래 추가
```
script-security 2
up /etc/openvpn/update-resolv-conf
down /etc/openvpn/update-resolv-conf
```


/etc/openvpn/update-resolv-conf 상단에 아래 추가
```
export NEW_DNS1="8.8.8.8"
export NEW_DNS2="8.8.4.4"
```

아래 명령어 실행
```
systemctl enable openvpn-profile.service
```
