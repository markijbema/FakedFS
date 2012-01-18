For now this is just an idea, implementation has to follow ;)

In my tests I want to do

```
FakedFS.activate_with! {
  dir: {
    subdir: {
      file: "file content"
    },
    other_subdir: {
      empty_dir: {}
    }
  }  
}

# do stuff

FakedFS.deactivate!
```