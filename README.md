# EasyMaps MWM releases

Enhanced MWM data is distributed as GitHub Release assets.

- [mwm-10-18-2026](https://github.com/virbula/mwm/releases/tag/mwm-10-18-2026): raw mobile MWM files, canonical API companions, SHA256SUMS and data manifest.
- [catalog-10-18-2026](https://github.com/virbula/mwm/releases/tag/catalog-10-18-2026): signed catalog, generation manifest and mobile test setup.
- [latest-stable](https://github.com/virbula/mwm/releases/tag/latest-stable) and [latest-beta](https://github.com/virbula/mwm/releases/tag/latest-beta): catalog-pointer.json channel references.

Source date: 2026-10-18. Current coverage: Rhode Island and Connecticut. Each file has an exact byte size and SHA256; raw MWM files have no outer gzip. Asset names use underscores; the catalog records the native installed filename.

The catalog index uses the existing EasyMaps Ed25519 signing key, offline-map-release-1, accepted from revision 3. Clients must trust their independently pinned public key, verify the index signature, then verify its catalog/generation bindings and every downloaded asset.

Finished data packages are available for mobile integration tests. General production routing, TIGER address routing and country-scale acceptance remain pending. The dedicated MWM catalog schema is easymaps-mwm-catalog-v1; legacy PMTiles/SQLite installers must not install these files.

Map data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), available under the Open Database License. MWM generation uses CoMaps/Organic Maps tooling with EasyMaps enhancement sections.
