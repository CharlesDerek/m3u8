# M3U8

M3U8 - a mini M3U8 downloader written in Golang for downloading and merging TS(Transport Stream) files.

You only need to specify the flags(`u`, `o`, `c`) to run, downloader will automatically download all TS files and consolidate them into a single TS file.

[中文说明](README_zh-CN.md)

## Features

- Download and parse M3U8（VOD）
- Retry on download TS failure
- Parse Master playlist
- Decrypt TS
- Merge TS

## Usage

### source

```bash
go run main.go -u=http://example.com/index.m3u8 -o=/data/example
```

### binary:

Linux & MacOS

```
./m3u8 -u=http://example.com/index.m3u8 -o=/data/example
```

Windows PowerShell

```
.\m3u8.exe -u="http://example.com/index.m3u8" -o="D:\data\example"
```

## Download

[Binary packages](https://github.com/charlesderek/m3u8/releases)

## Screenshots

![Demo](./screenshots/demo.gif)

## References

- [Example File Action(s)](https://go.dev/src/os/example_test.go)
- [Documentation](https://pkg.go.dev/os)
- [M3U8 - Wikipedia](https://stackoverflow.com/questions/33108105/converting-an-hls-m3u8-to-mp4)
- [MPEG transport stream - Wikipedia](https://en.wikipedia.org/wiki/MPEG_transport_stream)


## License

[MIT License](./LICENSE)