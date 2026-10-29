# 📸 Screenshot Inventory

Status of every image referenced by the main `README.md`.

## ✅ Already in this repo (real captures)

| File | Source | What it shows |
|---|---|---|
| `step-01-new-project-template.png` | EMSI workshop *"02 - Bootstrap ASP.NET 2022"* | *Create a new project* → `ASP.NET Web Application (.NET Framework)` template card |
| `step-02-create-webapp-empty-webforms.png` | same workshop | *Create an ASP.NET Web Application* wizard, **Vide/Empty** + **Web Forms** checked, project named `WebApplicationBootEMSI` |
| `step-03-solution-explorer-empty.png` | same workshop | Solution Explorer right after project creation (minimal — no pages yet) |
| `step-04-add-master-page.png` | same workshop | *Add New Item* → **Web Forms Master Page**, named `Site1.Master` |
| `step-05-nuget-bootstrap-install.png` | same workshop | NuGet Package Manager, Browse tab, `bootstrap 5.3.8`, Install button |
| `step-06-solution-explorer-after-bootstrap.png` | same workshop | Solution Explorer with `Content/` and `Scripts/` added after install |
| `step-07-master-page-design-view.png` | same workshop | `Site1.Master` in Design view, navbar links visible |
| `step-08-add-web-form-with-master.png` | same workshop | *Add New Item* → **Web Form with Master Page** |
| `step-09-select-master-page-dialog.png` | same workshop | *Select a Master Page* dialog, `Site1.Master` chosen |
| `step-10-content-page-design-view.png` | same workshop | Content page Design view merged with the Master Page |
| `step-14-browser-home.png` | **this repo, live** | `Default.aspx` rendered at desktop width (1280×900), via MSBuild + IIS Express + headless Chrome |
| `step-15-browser-navbar-collapsed.png` | **this repo, live** | `Default.aspx` at mobile width (390×844), navbar collapsed — captured over the Chrome DevTools Protocol |
| `step-15b-browser-navbar-open.png` | **this repo, live** | Same page, after an actual click on `.navbar-toggler` — menu open |
| `step-16-browser-webform1.png` | **this repo, live** | `webForm1.aspx` rendered at desktop width |
| `../demo-strip.png` | **this repo, live** | 4-panel composite of the four screenshots above |

The "live" captures were produced with:

```powershell
# Build
& "C:\Program Files\Microsoft Visual Studio\18\Insiders\MSBuild\Current\Bin\amd64\MSBuild.exe" `
  WebApplicationBootEMSI.csproj /p:Configuration=Debug

# Serve
& "C:\Program Files\IIS Express\iisexpress.exe" /path:"<project folder>" /port:52345

# Render + screenshot (headless Chrome, isolated temp profile, driven over CDP WebSocket)
& "C:\Program Files\Google\Chrome\Application\chrome.exe" --headless=new --remote-debugging-port=9477 ...
```

## ⏳ Not included — need a live, interactive desktop session

These four require actually clicking through a running Visual Studio instance on a real screen
(installer UI, a paused debugger, a build output pane, a terminal mid-`git push`). No automation
available in this environment can safely drive another app's GUI without taking over your actual
desktop session, so they were intentionally skipped rather than faked.

| # | File to add | What to capture |
|---|---|---|
| 1 | `step-vs-installer-workload.png` | Visual Studio Installer, **ASP.NET and web development** workload checked |
| 2 | `step-debug-breakpoint.png` | Breakpoint hit in `Site1.master.cs` → `Page_Load`, yellow debug arrow visible |
| 3 | `step-release-build-output.png` | *Output* window after **Build Solution** in `Release` configuration, "Build succeeded" |
| 4 | `step-git-push.png` | Terminal/PowerShell showing `git push` succeeding against GitHub |

**Recommended tools:** [ScreenToGif](https://www.screentogif.com/) or Win+Shift+S for stills.
Drop each file at the path above and it's already wired into the "Part H" section of the main
README (add an image reference there once captured).
