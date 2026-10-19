# CMSBundle for AWT

**Create your website. Shape your content. Manage it all in one place.**

CMSBundle brings the core Advanced Web Tools CMS packages together in a single installation. From visual page building and media management to themes and team accounts, it gives you a connected foundation for creating and maintaining your website.

## From first page to everyday publishing

- **Build visually.** Design responsive pages with Quill, reuse components and manage drafts and published content.
- **Keep media close.** Organize images, videos and documents in MediaLibrary, then select assets inside Quill through QuillMediaBridge.
- **Make the site your own.** Use ThemeEngine to choose your site's theme and customize its settings and layout. QuillThemeBridge connects theme resources to the visual editor.
- **Manage your team.** AccountManager brings profiles, account administration and permission management into the Dashboard.
- **Maintain your workspace.** Access package management and settings alongside your content tools.

## One bundle, connected tools

| Included package | Purpose |
| --- | --- |
| Dashboard | The administration workspace for your website. |
| Quill | Visual page building, reusable components and publishing tools. |
| MediaLibrary | A central library for uploading, browsing and organizing media. |
| QuillMediaBridge | MediaLibrary integration for Quill's media pickers. |
| ThemeEngine | Site theme selection, settings and layout customization. |
| QuillThemeBridge | Connects theme pages and components to Quill. |
| WelcomeTheme | An included starting theme. |
| AccountManager | User profiles, account administration and access management. |
| PackageManager | Package management within AWT. |
| SettingsManager | Settings management within AWT. |
| URPC | Structured document rendering used by the content tools. |

## A starting theme, automatically

On its first run, CMSBundle preserves an existing active theme. If none is active, it activates the first enabled theme registered with ThemeEngine. WelcomeTheme is included as a dependency to provide a starting point.

After activation, the public theme takes effect on the next request. You can then choose another theme through **Dashboard → Customization**.

## Get started

1. Install CMSBundle through the AWT package installer, allowing it to resolve the dependencies declared in the bundle manifest.
2. Open the Dashboard to access your content, media, accounts and administration tools.
3. Customize your theme and create your pages with Quill.

Requires **AWT 27.0.0 or later**. CMSBundle 1.0.0 declares ThemeEngine **1.0.4 or later** and the other included packages **1.0.0 or later**. Individual packages may have additional requirements.

## First-run behavior

CMSBundle records completed initialization with an `installed` file in its package directory. Once that file exists, it skips automatic theme selection on subsequent runs. If a theme is already active, it creates the marker without changing your selection. If no enabled theme is available, it leaves initialization pending and tries again on a later run.

The PHP process needs permission to create this marker in the package directory.

---

**CMSBundle 1.0.0** · By **ElStefanos** · Built for **Advanced Web Tools**
