# Use

#### Export and copy Zimbra Ldap


```ruby
su - zimbra -c "/opt/zimbra/libexec/zmslapcat -c /var/tmp"
scp /var/tmp/ldap.ldif root@remoteServer:/path
```


#### Parser ldif 

```ruby
./parser_ZimbraDistList ldap.ldif > zm_provision
```

#### Execute

```ruby
zmprov < zm_provision

```

#### Output file

```
cdl areasoftware@example.com
mdl areasoftware@example.com displayName 'Area Software'
adlm areasoftware@example.com fgarrido@example.com rrivas@example.com rgodoyg@example.com ggodoy@example.com pvarasc@example.com rburgos@example.com fcoronac@example.com fbersezio@example.com cvergaras@example.com uperez@example.com zsanhueza@example.com
```
