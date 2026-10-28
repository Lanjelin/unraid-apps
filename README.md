# Lanjelin's Unraid applications

Catalog metadata for Unraid Community Applications. Plugin source, installers, and releases remain in their respective project repositories.

## Applications

| Application | Type | Source and documentation | Support |
| --- | --- | --- | --- |
| unraid-icons | Plugin | [Shared icon library for Unraid VMs and Docker containers](https://github.com/Lanjelin/unraid-icons) | [Plugin issues](https://github.com/Lanjelin/unraid-icons/issues) |

The unraid-icons listing points directly to its existing self-contained plugin manifest. This repository does not rebuild or copy the plugin.

## Community Applications submission

This repository is prepared for submission; publication requires approval by Community Applications.

1. Open https://ca.unraid.net/submit/new and sign in with an Unraid account.
2. Add `https://github.com/Lanjelin/unraid-apps` as the repository.
3. Run **Validate**, then **Scan**. Resolve any reported issues and check the listing preview.
4. Submit for review. Plugin submissions are manually reviewed; approved listings appear after the next catalog build.

Until approved, install unraid-icons using the [project's manual installation instructions](https://github.com/Lanjelin/unraid-icons#install).

## Maintenance

- `ca_profile.xml` contains repository overview and support metadata.
- `plugins/` contains one XML wrapper per plugin, with `PluginURL` pointing to its published `.plg` manifest.
- For future Docker apps, add one XML template per app under `templates/`, with `Repository` pointing to its published container image and `TemplateURL` pointing to that template's raw GitHub URL.
- Keep application descriptions, icons, project links, and support links current.
- Publish plugin updates in the plugin's source repository. An unchanged manifest URL does not require a catalog edit for each release.
- After meaningful XML changes, rerun **Validate** and **Scan** in the submission portal.

Report catalog metadata problems in [this repository's issue tracker](https://github.com/Lanjelin/unraid-apps/issues). Report plugin behavior or installation problems in the application's support tracker above.

Format references: [submission requirements](https://ca.unraid.net/submit/help), [XML format](https://ca.unraid.net/submit/help/repository-xml), and [supported XML fields](https://ca.unraid.net/submit/help/xml-field-reference).

## License

Catalog metadata and documentation are licensed under the [MIT License](LICENSE). Applications and third-party icons retain their respective licenses and trademark rights.
