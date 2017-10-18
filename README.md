```
     /\     (_)       
    /  \     _   _ __ 
   / /\ \   | | | '__|
  / ____ \  | | | |   
 /_/    \_\ |_| |_|   
 
Live reload for Go apps
```

[![CircleCI](https://circleci.com/gh/cosmtrek/air/tree/master.svg?style=shield)](https://circleci.com/gh/cosmtrek/air/tree/master)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/4885b8dddaa540f9ae6fe850b4611b7b)](https://www.codacy.com/app/cosmtrek/air?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=cosmtrek/air&amp;utm_campaign=Badge_Grade)

![air](docs/air.png)

## Motivation

When I get started with developing websites in Go and [gin](https://github.com/gin-gonic/gin) framework, it's a pity 
that gin lacks live-reloading function. In fact, I tried [fresh](https://github.com/pilu/fresh) and it seems not much 
flexible, so I intended to rewrite it in a better way. Finally, Air's born. 
In addition, great thanks to [pilu](https://github.com/pilu), no fresh, no air :)

Air is a terminal command for live-reloading Go applications. Just `air` in your project root directory, leave it alone,
and focus on your code.

## Installation

```bash
go get github.com/cosmtrek/air
```

## Usage

First enter into your project

```bash
cd /path/to/your_project
```

The simplest usage is run

```bash
# firstly find `.air.conf` in current directory, if not found, use defaults
air
```

While I prefer the second way

```bash
# 1. create a new file
touch .air.conf

# 2. paste `air.conf.example` into this file, and modify it to satisfy your needs

# 3. run air with your configs. If file name is `.air.conf`, just run `air`
air -c .air.conf
```

See the complete [air.conf.example](air.conf.example)

### Debug

`air -d` prints all logs.

## Contributing

PRs are welcome~

## License

[GNU General Public License v3.0](LICENSE)