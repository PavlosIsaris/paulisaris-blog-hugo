# About

This is the code repository for my blog. The posts are written in Markdown and the blog
uses [Hugo](https://gohugo.io/getting-started/).

## Installation

In order to install the used Hugo theme, run the following command:

```bash
git submodule update --init --recursive
```

## Compiling & Running the server

### Docker option (recommended)

The Hugo server is running in a Docker container. To start the server:

```bash
docker-compose up
```

The output will be like:

```text
docker compose up                                                               1 ✘ 
[+] Running 4/4
 ⠿ server Pulled                                                                                                                           3.9s
   ⠿ b4a6e23922dd Pull complete                                                                                                            0.8s
   ⠿ 91dbce0c9c11 Pull complete                                                                                                            1.8s
   ⠿ 361df89f5866 Pull complete                                                                                                            1.9s
[+] Running 1/1
 ⠿ Container 026bcc688ade_paulisaris-blog-hugo-server-1  Recreated                                                                         0.3s
Attaching to paulisaris-blog-hugo-server-1
paulisaris-blog-hugo-server-1  | Building sites … 
paulisaris-blog-hugo-server-1  |                    | EN  
paulisaris-blog-hugo-server-1  | +------------------+----+
paulisaris-blog-hugo-server-1  |   Pages            | 55  
paulisaris-blog-hugo-server-1  |   Paginator pages  |  5  
paulisaris-blog-hugo-server-1  |   Non-page files   |  0  
paulisaris-blog-hugo-server-1  |   Static files     | 40  
paulisaris-blog-hugo-server-1  |   Processed images |  0  
paulisaris-blog-hugo-server-1  |   Aliases          | 16  
paulisaris-blog-hugo-server-1  |   Sitemaps         |  1  
paulisaris-blog-hugo-server-1  |   Cleaned          |  0  
paulisaris-blog-hugo-server-1  | 
paulisaris-blog-hugo-server-1  | Total in 244 ms
paulisaris-blog-hugo-server-1  | Watching for changes in /src/{content,data,layouts,static,themes}
paulisaris-blog-hugo-server-1  | Watching for config changes in /src/config.toml
paulisaris-blog-hugo-server-1  | Environment: "development"
paulisaris-blog-hugo-server-1  | Serving pages from memory
paulisaris-blog-hugo-server-1  | Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
paulisaris-blog-hugo-server-1  | Web Server is available at http://localhost:1313/ (bind address 0.0.0.0)
paulisaris-blog-hugo-server-1  | Press Ctrl+C to stop

```

It will build the website and start the server and you can access it at `http://localhost:1313`.

### Non-Docker option

You need to have Huge version `0.54.0` installed. You can download it from
the [official website](https://gohugo.io/getting-started/installing/).

To start the server:

```bash
hugo server
```

To build the static pages:

```bash
hugo
```
