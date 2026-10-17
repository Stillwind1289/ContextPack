# PromptPack

Bundle selected project files into one AI-ready context block with a single command.

## First version

- Select files in the VS Code Explorer and run **PromptPack: Copy Selected Files for AI**.
- The selected text files are copied to your clipboard with their relative paths as headings.
- `.env` files, common key files, paths containing `node_modules` or `.git`, binary files, files over 30 KB, and bundles over 100,000 characters are skipped.
- Files are processed locally by the extension. PromptPack does not send them to an external server.

## How to use

1. Open a project in VS Code.
2. Select one or more files in the Explorer.
3. Right-click and choose **PromptPack: Copy Selected Files for AI**.
4. Paste the copied context into your AI chat.

You can also run the command from the Command Palette. If no files are selected, PromptPack uses the active editor file.

## Safety note

The sensitive-file filter is a precaution, not a guarantee. Review the copied content before sharing it with any AI service. Never select or share secrets intentionally.

## Development

Requirements: Node.js and npm.

```bash
npm install
npm run compile
```

## Before publishing

- Replace `REPLACE_WITH_YOUR_PUBLISHER_ID` in `package.json` with your actual VS Code Marketplace publisher ID.
- Test the extension in VS Code.
- Review the README, name, icon, license, and privacy behaviour.
- Update the version number for future releases.

## License

MIT
