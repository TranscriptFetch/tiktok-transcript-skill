<p align="center">
  <img src="https://raw.githubusercontent.com/TranscriptFetch/tiktok-transcript-skill/main/assets/logo.png" alt="TranscriptFetch" width="84" height="84" />
</p>

# TikTok Transcript Skill

An agent skill that gives Claude Code, Codex, Cursor and other AI agents TikTok transcripts, through the [TranscriptFetch](https://transcriptfetch.com/?utm_source=github&utm_medium=skill&utm_campaign=tiktok-transcript-skill) API.

- **Transcripts** of any public TikTok video, with timestamps, from its captions or by AI transcription when it has none
- **Find videos** by search, profile or playlist, with paging
- **Many at once**: up to 50 transcripts per request, or a whole profile
- **Ready for AI**: plain text (about two-thirds fewer tokens), Markdown with timestamp links, or chunks sized for embeddings

## Install

```bash
npx skills add TranscriptFetch/tiktok-transcript-skill
```

Or copy the one file into Claude Code yourself:

```bash
mkdir -p ~/.claude/skills/tiktok-transcript
curl -fsSL https://raw.githubusercontent.com/TranscriptFetch/tiktok-transcript-skill/main/skills/tiktok-transcript/SKILL.md -o ~/.claude/skills/tiktok-transcript/SKILL.md
```

For other agents, put [`skills/tiktok-transcript/SKILL.md`](skills/tiktok-transcript/SKILL.md) in that agent's skills folder.

## First run

The first time you ask for a transcript, the agent opens a TranscriptFetch page in your browser. Sign in, check the code and click Approve. The agent gets its own API key, which never appears in the chat and which you can revoke on your API Keys page. No key to copy, no password shared with the agent.

## Try

- "What does this TikTok say? https://www.tiktok.com/@.../video/..."
- "Transcribe this TikTok and rewrite the hook three ways."
- "Pull the last 30 videos from @creator with transcripts and list the topics they cover."
- "Search TikTok for videos about meal prep and summarize the common advice."

## Cost

50 free credits every month, no card. 1 credit per caption transcript and per listing page; AI transcription of a video without captions is 1 credit per started 5 minutes of audio. Failed requests are free. Plans: [transcriptfetch.com/pricing](https://transcriptfetch.com/pricing?utm_source=github&utm_medium=skill&utm_campaign=tiktok-transcript-skill).

## Other platforms

- [YouTube Transcript Skill](https://github.com/TranscriptFetch/youtube-transcript-skill)
- [Instagram Transcript Skill](https://github.com/TranscriptFetch/instagram-transcript-skill)
- [MCP server](https://github.com/TranscriptFetch/youtube-tiktok-instagram-transcript-mcp) for YouTube, TikTok and Instagram transcripts in any MCP client
- [API docs](https://transcriptfetch.com/docs?utm_source=github&utm_medium=skill&utm_campaign=tiktok-transcript-skill)

## License

MIT
