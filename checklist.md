### Misc
1. Use git bash (not powershell)
1. `find "C:\code\revealjs-elasticsearch\reviews" -type f -exec curl -XPOST http://localhost:9200/pitt_talk/review --data-binary "@{}" \;`

### When you get there
1. Get on wifi
1. Make sure es docker image is running fine (switch to IC VM if needed)
1. Make sure local indices are gone
1. Delete any if needed `curl -XDELETE http://localhost:9200/pitt_talk`
1. Open presentation and scroll through
1. Once connected to projector - use the notes on the laptop







