> [!IMPORTANT]
>
> Thank you for accessing this project.
>
> Because this is used by a large number of users, it may stop due to Deno
> Deploy quota limit.
>
> If you want to recieve RSS feed of your posts, you can use official RSS:
> `https://bsky.app/profile/__bsky-handle__/rss`

# Bluestream

RSS feed generator for [Bluesky](https://bsky.app).

<https://bluestream.deno.dev/>

## Development

This works with [Deno](https://deno.land).

To run this locally, clone this repository and create `.env` file with the
following content:

```shell
BLUESKY_IDENTIFIER=your-handle
BLUESKY_PASSWORD=your-pass
```

After that, run `deno task dev` to start server.

## Author

[kawarimidoll](https://bsky.app/profile/did:plc:okalufxun5rpqzdrwf5bpu3d)

## License

MIT

## MAR local

In genMainContent() (in server.ts), ignore image and strip P tag in CDATA output.
I'm using this tool output for the trigger in IFTTT (not for human being); some HTML tags may cause some unwanted result in connected application.