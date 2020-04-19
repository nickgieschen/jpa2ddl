# Developers guide

## Releasing the new version

```shell
mvn release:clean
mvn release:prepare
mvn release:perform
git pushtags
git add README.md
git commit -m "Readme version update"
git push
```

## Pushing to github mvn repo
Make sure github creds in ~/.m2/settings.xml
```
<settings>
  <servers>
    <server>
      <id>github</id>
      <username>[username]</username>
      <password>[password]</password>
    </server>
  </servers>
</settings>
```
`mvn clean deploy`
