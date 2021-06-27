# iSSH2

A fork of [Frugghi/iSSH2][] with the following modifications:

- Install `*.pc` files alongside libraries to allow packages such as
  [libgit2][] to correctly link against libssh2.

- Instead of building universal libraries that contain slices for both iOS and
  iOS Simulator, add `iphonesimulator` as a distinct platform in order to
  support bundling an `.xcframework`. Used by [sharplet/swift-cgit2][] to
  distribute libgit2 as a Swift package.

Licensed under the same terms as [Frugghi/iSSH2][]; see [LICENSE](/LICENSE).

[Frugghi/iSSH2]: https://github.com/Frugghi/iSSH2
[libgit2]: https://github.com/libgit2/libgit2
[sharplet/swift-cgit2]: https://github.com/sharplet/swift-cgit2
