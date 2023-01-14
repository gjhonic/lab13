# Laboratory work №13

**Install Projects**

```bash
git clone git@github.com:gjhonic/lab12.git
```

**Install Ngnix**

```bash
# Install Nginx
sudo pacman -S nginx

# Configure Nginx
curl https://raw.githubusercontent.com/gjhonic/lab13/main/proxy/todos.conf | sudo tee /etc/nginx/nginx.conf > /dev/null

# Restart Nginx (not work in windows wsl)
sudo systemctl restart nginx

#if you use windows wsl then need command
sudo service nginx start
```

**launch**

```bash
$ cd lab13
$ cargo run
```

**Test**

```bash
$ curl http://127.0.0.1/v1/todos/{your_guid}
> {"assigned":"user@example.com","id":"{your_guid}","message":"Test message","priority":"A"}
```