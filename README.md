# GUIDE use tsrc

## Requirements
- Python version 3

## Setup

Create the workspace
```
mkdir pbl6
cd pbl6
```

Install `tsrc` tool - help manage many repos
```
pip install tsrc
tsrc init git@github.com:hovanvydut/pbl6.git
```

Synchronize all the repositories in the workspace (git pull):
```
tsrc sync
```

Checkout all repo of group BE to main branch
```
tsrc foreach -g be -- git checkout main
```

Use `tsrc foreach -g be -- <command>`

## References

* https://your-tools.github.io/tsrc/