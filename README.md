# sample-unity-project
[itch.io link](https://popcron.itch.io/sample-unity-game)

### Initial setup
0. Setup `ITCH_USER`, `ITCH_GAME` variables and the `BUTLER_CREDENTIALS` secret in the repo's settings. The secret is generated [here](https://itch.io/user/settings/api-keys) and the other two keys build the itch.io url
1. Copy the .github folder over to the repo (this will be 2 .yaml workflow files)
2. Update the main.yaml file's `PROJECT_DIR` value, by default it points to `Sample Unity Project` from the root, if your assets folder is at the root you should use `/` instead
3. Push everything and run the activation workflow to get a license file, then convert the generated license file using [this site](https://license.unity3d.com/manual)
  the contents of the file will be the `UNITY_LICENSE` secret in your repo's settings (if you have a pro license activation is a bit difference, see [this](https://game.ci/docs/github/activation/))
4. A build will be triggered on any push or manual dispatch

### When builds happen
Builds happen by manually dispatching through the actions tab, or if a tag is pushed
