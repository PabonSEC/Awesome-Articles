<div align="center">
    <img src="https://img.icons8.com/color/100/000000/git.png">
    <h1>
      Git Commands
    </h1>
</div>

## Save username and password in GIT

### Run

```bash
git config --global credential.helper store
```

After running this command, when you **push** to your repository or **pull** from your repository, you'll get asked `username` and `password` for first time.

Then credentials will be stored into your home directory named `.git-credentials` file in plaintext.

You can use this command to store your credentials into cache memory for specific time(in seconds).

```bash
git config --global credential.helper 'cache --timeout=14400'
```

This command will remember your credentials for 4 hours. Your `username` and `password` will be asked for the first time during **push** or **pull** as well.
