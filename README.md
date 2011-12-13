
## rubygems_cache
    
```bash
  $ mkdir ~/installed
  $ git clone git@github.com:akitaonrails/rubygems_proxy.git ~/installed/
```

## nginx for rubygems_cache

  install passenger with nginx, then:

```bash
  $ rm -rf /opt/nginx/conf
  $ ln -s $DOTFILES_PATH/conf/nginx /opt/nginx/conf
```

## magnet protocol (ktorrent)

```bash
  gconftool-2 -t string -s /desktop/gnome/url-handlers/magnet/command "/usr/bin/ktorrent %s"
  gconftool-2 -s /desktop/gnome/url-handlers/magnet/needs_terminal false -t bool
  gconftool-2 -t bool -s /desktop/gnome/url-handlers/magnet/enabled true
```
