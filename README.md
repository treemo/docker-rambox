# install

```
mkdir -p $HOME/docker-data/rambox/config $HOME/docker-data/rambox/share
docker run \
        -d \
        -e LANG \
        -e LANGUAGE \
        -e LC_ALL \
        -e DISPLAY \
        -v /tmp/.X11-unix:/tmp/.X11-unix:ro \
        -v $HOME/docker-data/rambox/config:/home/user/.config/Rambox \
        -v $HOME/docker-data/rambox/share:/home/user/docker \
        --name rambox \
        treemo/rambox
```
