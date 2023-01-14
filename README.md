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

# Restart Nginx
sudo systemctl restart nginx
```

**launch**

```bash
$ cd lab13
$ cargo run
```