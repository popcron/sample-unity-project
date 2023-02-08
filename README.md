# sample-unity-project
[itch.io link]([https://itch.io/popcron/sample-unity-game](https://popcron.itch.io/sample-unity-game)

### Initial setup
1. Run the activation workflow to get a license file, then convert the generated license file using [this site](https://license.unity3d.com/manual)
  the contents of the file should be the `UNITY_LICENSE` secret in your repo's settings
2. The `BUTLER_CREDENTIALS` secret should also be a butler API key that can be retrieved [from here](https://itch.io/user/settings/api-keys)
3. The `ITCH_USER` and `ITCH_GAME` variables (under the same area where secrets are set) should match your itch.io project's url (`...itch.io/popcron/sample-unity-game`)

### When builds happen
Builds happen by manually dispatching through the actions tab, or if a tag is pushed
