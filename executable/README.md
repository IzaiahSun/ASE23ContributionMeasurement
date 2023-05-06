# executable binary

We provided a docker environment to run the tool. We only provided a executable binary during review period, it will be open-sourced upon acceptance.

## How to use

```shell
# First build the docker
docker build -t contribution .

# Then run it, replace the {proj_name} with the name of project, the result will be saved at /path/to/git/repo/output.json
docker run -v /path/to/git/repo:/script/projects/{proj_name} contribution /script/analyze projects/{proj_name} output.json
```

## Other notice

This tool is not optimized for space consumption and may generate a lot of temporary files during running. It will take up a lot of disk space. If you don't have enough disk space, please pick some small projects.
