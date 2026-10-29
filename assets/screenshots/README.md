# 📸 Screenshot & GIF Checklist

The main `README.md` references the image files listed below. They are **not included in this
repository** (this environment cannot drive Visual Studio's GUI or a browser to capture them).
Follow this checklist to produce them yourself — it only takes a few minutes — then drop each
file at the exact path shown. GitHub will pick them up automatically since the README already
points at these paths.

**Recommended tools:** [ScreenToGif](https://www.screentogif.com/) (Windows, free, screenshots *and* GIFs) or the Win+Shift+S Snipping Tool for stills.

**Recommended size:** keep screenshots ≤ 1600 px wide and compress GIFs (ScreenToGif's built-in
optimizer or [ezgif.com](https://ezgif.com/)) so the README stays fast to load.

| # | File to create | What to capture |
|---|---|---|
| 1 | `assets/screenshots/step-01-vs-installer-workload.png` | Visual Studio Installer, **ASP.NET and web development** workload checked |
| 2 | `assets/screenshots/step-02-new-project-search.png` | *Create a new project* dialog, search box filled with `ASP.NET Web Application` |
| 3 | `assets/screenshots/step-03-configure-project.png` | *Configure your new project* dialog (name/location/solution name) |
| 4 | `assets/screenshots/step-04-webforms-template.png` | *Create a new ASP.NET Web Application* wizard with **Web Forms** selected |
| 5 | `assets/screenshots/step-05-solution-explorer.png` | Solution Explorer showing the freshly generated project tree |
| 6 | `assets/screenshots/step-06-nuget-manage-packages.png` | *Manage NuGet Packages for Solution* window, Browse tab |
| 7 | `assets/screenshots/step-07-nuget-bootstrap-install.png` | Bootstrap package selected (`5.3.8`) with the **Install** button visible |
| 8 | `assets/screenshots/step-08-content-scripts-folders.png` | Solution Explorer with `Content/` and `Scripts/` expanded after install |
| 9 | `assets/screenshots/step-09-sitemaster-markup.png` | `Site1.Master` open in the editor, navbar markup visible |
| 10 | `assets/screenshots/step-10-default-aspx-markup.png` | `Default.aspx` open in the editor |
| 11 | `assets/screenshots/step-11-add-web-form-dialog.png` | *Add New Item* → *Web Form* dialog, name set to `webForm1.aspx` |
| 12 | `assets/screenshots/step-12-set-as-start-page.png` | Solution Explorer context menu with **Set as Start Page** highlighted |
| 13 | `assets/screenshots/step-13-run-iis-express.png` | Visual Studio toolbar with the green ▶ **IIS Express** run button visible |
| 14 | `assets/screenshots/step-14-browser-home.png` | Running site — `Default.aspx` in the browser, desktop width |
| 15 | `assets/screenshots/step-15-browser-navbar-collapsed.png` | Running site — browser narrowed to show the collapsed Bootstrap navbar (hamburger icon) |
| 16 | `assets/screenshots/step-16-browser-webform1.png` | Running site — `webForm1.aspx` page (the "Contacts" link) |
| 17 | `assets/screenshots/step-17-debug-breakpoint.png` | Breakpoint hit in `Site1.master.cs` → `Page_Load`, yellow debug arrow visible |
| 18 | `assets/screenshots/step-18-release-build-output.png` | *Output* window after **Build Solution** in `Release` configuration, "Build succeeded" |
| 19 | `assets/screenshots/step-19-git-push.png` | Terminal/PowerShell showing `git push` succeeding against GitHub |
| 20 | `assets/demo.gif` | Short screen recording: launch (F5) → home page loads → resize window to show responsive navbar → click **Contacts** → close |

Once the files are in place, delete this checklist file (or keep it for the next contributor).
