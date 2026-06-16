This file is a merged representation of the entire codebase, combined into a single document by Repomix.
The content has been processed where line numbers have been added, content has been formatted for parsing in markdown style.

# File Summary

## Purpose
This file contains a packed representation of the entire repository's contents.
It is designed to be easily consumable by AI systems for analysis, code review,
or other automated processes.

## File Format
The content is organized as follows:
1. This summary section
2. Repository information
3. Directory structure
4. Repository files (if enabled)
5. Multiple file entries, each consisting of:
  a. A header with the file path (## File: path/to/file)
  b. The full contents of the file in a code block

## Usage Guidelines
- This file should be treated as read-only. Any changes should be made to the
  original repository files, not this packed version.
- When processing this file, use the file path to distinguish
  between different files in the repository.
- Be aware that this file may contain sensitive information. Handle it with
  the same level of security as you would the original repository.

## Notes
- Some files may have been excluded based on .gitignore rules and Repomix's configuration
- Binary files are not included in this packed representation. Please refer to the Repository Structure section for a complete list of file paths, including binary files
- Files matching patterns in .gitignore are excluded
- Files matching default ignore patterns are excluded
- Line numbers have been added to the beginning of each line
- Content has been formatted for parsing in markdown style
- Files are sorted by Git change count (files with more changes are at the bottom)

# Directory Structure
```
.gitignore
astro.config.mjs
old-site/CIS_Syllabi.html
old-site/cis241.html
old-site/cis266.html
old-site/cis296.html
old-site/css/styles.css
old-site/index.html
old-site/projects.html
old-site/projects/CRUD-RESTful-service.html
old-site/projects/godot-roguelike.html
old-site/projects/RESTful-AJAX-JSON-PHP-MySQL.html
old-site/projects/simple-forum.html
old-site/projects/sportspro.html
old-site/projects/switcher.html
old-site/projects/voting-system.html
old-site/projects/wcf.html
package.json
public/documents/JaredStreetResume.pdf
public/documents/syllabi/CIS130_syllabus.pdf
public/documents/syllabi/CIS131_syllabus.pdf
public/documents/syllabi/CIS137_syllabus.pdf
public/documents/syllabi/CIS194_syllabus.pdf
public/documents/syllabi/CIS195_syllabus.pdf
public/documents/syllabi/CIS196_syllabus.pdf
public/documents/syllabi/CIS207_syllabus.pdf
public/documents/syllabi/CIS225_syllabus.pdf
public/documents/syllabi/CIS236_syllabus.pdf
public/documents/syllabi/CIS241_syllabus.pdf
public/documents/syllabi/CIS248_syllabus.pdf
public/documents/syllabi/CIS266_syllabus.pdf
public/documents/syllabi/CIS279_syllabus.pdf
public/documents/syllabi/CIS293_syllabus.pdf
public/documents/syllabi/CIS296_syllabus.pdf
public/favicon.ico
public/favicon.svg
public/screenshots/darksouls-database-display-API.png
public/screenshots/darksouls-home.png
public/screenshots/darksouls-live-table.png
public/screenshots/display-switcher-apply.png
public/screenshots/display-switcher-list.png
public/screenshots/display-switcher-show.png
public/screenshots/library-console-menu.png
public/screenshots/library-console-output.png
public/screenshots/library-wcf-service-browser.png
public/screenshots/realtime-voting-home.png
public/screenshots/realtime-voting-results.png
public/screenshots/RESTful-AJAX-display-all.png
public/screenshots/RESTful-AJAX-display-one.png
public/screenshots/RESTful-AJAX-home.png
public/screenshots/roguelike-combat-floor.png
public/screenshots/roguelike-end-screen.png
public/screenshots/roguelike-final-floor.png
public/screenshots/roguelike-reward-selection.png
public/screenshots/roguelike-start-menu.png
public/screenshots/simple-forum-create-post.png
public/screenshots/simple-forum-home.png
public/screenshots/simple-forum-view-post.png
public/screenshots/Slide1.PNG
public/screenshots/Slide2.PNG
public/screenshots/Slide3.PNG
public/screenshots/Slide4.PNG
public/screenshots/Slide5.PNG
public/screenshots/Slide6.PNG
public/screenshots/Slide7.PNG
public/screenshots/sportspro-home.png
public/screenshots/sportspro-incidents.png
public/screenshots/sportspro-technician-incidents.png
public/screenshots/tempheadshot.ARW
public/screenshots/tempheadshot.jpeg
README.md
src/components/Footer.astro
src/components/Nav.astro
src/layouts/BaseLayout.astro
src/pages/coursework.astro
src/pages/index.astro
src/pages/projects/crud-restful-service.astro
src/pages/projects/display-switcher.astro
src/pages/projects/godot-roguelike.astro
src/pages/projects/index.astro
src/pages/projects/rest-ajax-php.astro
src/pages/projects/simple-forum.astro
src/pages/projects/sportspro.astro
src/pages/projects/voting-system.astro
src/pages/projects/wcf.astro
src/styles/global.css
tsconfig.json
```

# Files

## File: src/pages/coursework.astro
````astro
  1: ---
  2: import BaseLayout from "../layouts/BaseLayout.astro";
  3: 
  4: const courseTracks = [
  5:   {
  6:     title: "Programming Foundations",
  7:     description:
  8:       "Core programming courses covering C#, introductory programming concepts, data analysis, and secure coding practices.",
  9:     courses: ["CIS 130", "CIS 131", "CIS 137", "CIS 225"],
 10:   },
 11:   {
 12:     title: "Web Development",
 13:     description:
 14:       "Coursework focused on PHP, dynamic websites, ASP.NET, web services, and application development.",
 15:     courses: ["CIS 195", "CIS 196", "CIS 236", "CIS 241", "CIS 266", "CIS 296"],
 16:   },
 17:   {
 18:     title: "Databases and Business Systems",
 19:     description:
 20:       "Database and business technology courses covering relational data, eBusiness, and database-backed systems.",
 21:     courses: ["CIS 194", "CIS 207", "CIS 279"],
 22:   },
 23:   {
 24:     title: "Advanced Development",
 25:     description:
 26:       "Upper-level courses focused on larger development projects, new technologies, and applied software work.",
 27:     courses: ["CIS 248", "CIS 293"],
 28:   },
 29: ];
 30: 
 31: const syllabi = [
 32:   {
 33:     code: "CIS 130",
 34:     title: "Introduction to Programming",
 35:     href: "/documents/syllabi/CIS130_syllabus.pdf",
 36:     area: "Programming Foundations",
 37:   },
 38:   {
 39:     code: "CIS 131",
 40:     title: "C# Programming",
 41:     href: "/documents/syllabi/CIS131_syllabus.pdf",
 42:     area: "C# / .NET",
 43:   },
 44:   {
 45:     code: "CIS 137",
 46:     title: "Data Analysis",
 47:     href: "/documents/syllabi/CIS137_syllabus.pdf",
 48:     area: "Data",
 49:   },
 50:   {
 51:     code: "CIS 194",
 52:     title: "Introduction to Databases",
 53:     href: "/documents/syllabi/CIS194_syllabus.pdf",
 54:     area: "Databases",
 55:   },
 56:   {
 57:     code: "CIS 195",
 58:     title: "Internet Programming Essentials",
 59:     href: "/documents/syllabi/CIS195_syllabus.pdf",
 60:     area: "Web Development",
 61:   },
 62:   {
 63:     code: "CIS 196",
 64:     title: "Internet Programming II",
 65:     href: "/documents/syllabi/CIS196_syllabus.pdf",
 66:     area: "Web Development",
 67:   },
 68:   {
 69:     code: "CIS 207",
 70:     title: "eBusiness",
 71:     href: "/documents/syllabi/CIS207_syllabus.pdf",
 72:     area: "Business Systems",
 73:   },
 74:   {
 75:     code: "CIS 225",
 76:     title: "Secure Programming",
 77:     href: "/documents/syllabi/CIS225_syllabus.pdf",
 78:     area: "Security",
 79:   },
 80:   {
 81:     code: "CIS 236",
 82:     title: "Introduction to MS Web Development",
 83:     href: "/documents/syllabi/CIS236_syllabus.pdf",
 84:     area: "ASP.NET",
 85:   },
 86:   {
 87:     code: "CIS 241",
 88:     title: "Dynamic Website Development",
 89:     href: "/documents/syllabi/CIS241_syllabus.pdf",
 90:     area: "PHP / MySQL",
 91:   },
 92:   {
 93:     code: "CIS 248",
 94:     title: "Advanced Application Development",
 95:     href: "/documents/syllabi/CIS248_syllabus.pdf",
 96:     area: "Application Development",
 97:   },
 98:   {
 99:     code: "CIS 266",
100:     title: "Web Services",
101:     href: "/documents/syllabi/CIS266_syllabus.pdf",
102:     area: "APIs / Services",
103:   },
104:   {
105:     code: "CIS 279",
106:     title: "Databases II",
107:     href: "/documents/syllabi/CIS279_syllabus.pdf",
108:     area: "Databases",
109:   },
110:   {
111:     code: "CIS 293",
112:     title: "Advanced Technologies",
113:     href: "/documents/syllabi/CIS293_syllabus.pdf",
114:     area: "Tools / Automation",
115:   },
116:   {
117:     code: "CIS 296",
118:     title: "MS Web Development II",
119:     href: "/documents/syllabi/CIS296_syllabus.pdf",
120:     area: "C# / ASP.NET Core",
121:   },
122: ];
123: ---
124: 
125: <BaseLayout
126:   title="Coursework & Syllabi | Jared Street"
127:   description="Coursework archive and CIS syllabi for Jared Street's programming, web development, database, and application development courses."
128: >
129:   <section class="page-hero fade-in">
130:     <p class="eyebrow">Coursework Archive</p>
131:     <h1>Coursework & Syllabi</h1>
132:     <p>
133:       A supporting archive of CIS coursework, course syllabi, and academic project
134:       context.
135:     </p>
136: 
137:     <div class="button-row">
138:       <a class="button button-primary" href="/projects/">View Projects</a>
139:       <a class="button button-secondary" href="/documents/JaredStreetResume.pdf">View Resume</a>
140:     </div>
141:   </section>
142: 
143:   <section class="fade-in">
144:     <div class="section-heading">
145:       <p class="eyebrow">Academic Focus</p>
146:       <h2>Course Areas</h2>
147:       <p>
148:         The coursework behind this portfolio covers programming, web development,
149:         databases, application development, services, and practical tooling.
150:       </p>
151:     </div>
152: 
153:     <div class="course-track-grid">
154:       {courseTracks.map((track) => (
155:         <article class="course-track-card">
156:           <h3>{track.title}</h3>
157:           <p>{track.description}</p>
158: 
159:           <div class="tech-list">
160:             {track.courses.map((course) => (
161:               <span class="tech-pill">{course}</span>
162:             ))}
163:           </div>
164:         </article>
165:       ))}
166:     </div>
167:   </section>
168: 
169:   <section class="section-card fade-in">
170:     <div class="section-heading">
171:       <p class="eyebrow">Syllabi</p>
172:       <h2>CIS Course Syllabi</h2>
173:       <p>
174:         PDF syllabi from completed or in-progress CIS courses. These are included
175:         as academic references, not as the primary focus of the portfolio.
176:       </p>
177:     </div>
178: 
179:     <div class="syllabus-grid">
180:       {syllabi.map((course) => (
181:         <article class="syllabus-card">
182:           <div>
183:             <p class="course-area">{course.area}</p>
184:             <h3>{course.code}</h3>
185:             <p>{course.title}</p>
186:           </div>
187: 
188:           <a
189:             class="text-link"
190:             href={course.href}
191:             target="_blank"
192:             rel="noopener noreferrer"
193:           >
194:             View Syllabus
195:           </a>
196:         </article>
197:       ))}
198:     </div>
199:   </section>
200: </BaseLayout>
````

## File: src/pages/projects/crud-restful-service.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const crudCode = `<?php
  6: 
  7: include_once('classes/Character.php');
  8: include_once('classes/Faction.php');
  9: include_once('classes/Weapon.php');
 10: include_once('classes/DB_200.php');
 11: 
 12: header('Content-Type: application/json');
 13: 
 14: $db = new DB_200();
 15: 
 16: $action = $_REQUEST['action'];
 17: $table = $_REQUEST['table'];
 18: 
 19: if ($action == "read") {
 20:     $id = !empty($_REQUEST['id']) ? $_REQUEST['id'] : null;
 21:     $result = $db->read($table, $id);
 22:     $data = [];
 23: 
 24:     while ($row = $result->fetch_assoc()) {
 25:         $data[] = $row;
 26:     }
 27: 
 28:     echo json_encode($data);
 29: }
 30: 
 31: if ($action == "insert") {
 32:     $data = $_POST;
 33:     unset($data['action'], $data['table']);
 34: 
 35:     $db->insert($table, $data);
 36:     echo json_encode(["status" => "inserted"]);
 37: }
 38: 
 39: if ($action == "update") {
 40:     $id = $_POST['id'];
 41:     $data = $_POST;
 42:     unset($data['action'], $data['table'], $data['id']);
 43: 
 44:     $db->update($table, $id, $data);
 45:     echo json_encode(["status" => "updated"]);
 46: }
 47: 
 48: if ($action == "delete") {
 49:     $id = $_REQUEST['id'];
 50: 
 51:     $db->delete($table, $id);
 52:     echo json_encode(["status" => "deleted"]);
 53: }
 54: ?>`;
 55: 
 56: const techStack = [
 57:   "PHP",
 58:   "MySQL",
 59:   "Object-Oriented PHP",
 60:   "JavaScript",
 61:   "jQuery AJAX",
 62:   "JSON",
 63:   "HTML",
 64:   "CSS",
 65: ];
 66: 
 67: const features = [
 68:   "Provides a PHP API endpoint for CRUD operations",
 69:   "Supports reading, inserting, updating, and deleting records",
 70:   "Uses a MySQL database named darksouls",
 71:   "Stores data in characters, factions, and weapons tables",
 72:   "Uses PHP classes for Character, Faction, Weapon, and database access logic",
 73:   "Returns API responses as JSON",
 74:   "Uses jQuery AJAX requests to communicate with the API",
 75:   "Displays live table data for characters, factions, and weapons",
 76:   "Includes form controls for CRUD operations on each table",
 77:   "Uses animation effects for inserted, updated, and deleted rows",
 78:   "Includes sound effects and Dark Souls-inspired UI styling",
 79:   "Includes an SQL export for recreating the database structure and sample data",
 80: ];
 81: 
 82: const screenshots = [
 83:   {
 84:     src: "/screenshots/darksouls-home.png",
 85:     alt: "Dark Souls CRUD web service home page",
 86:     title: "Dark Souls CRUD Home Page",
 87:     caption: "Client interface for the Dark Souls-themed CRUD web service.",
 88:   },
 89:   {
 90:     src: "/screenshots/darksouls-live-table.png",
 91:     alt: "Live database display",
 92:     title: "Live Table Viewer",
 93:     caption: "CRUD operations are reflected in the live table display.",
 94:   },
 95:   {
 96:     src: "/screenshots/darksouls-database-display-API.png",
 97:     alt: "Entire database displayed through the API",
 98:     title: "Database API Display",
 99:     caption: "Database records returned through the PHP API.",
100:   },
101: ];
102: ---
103: 
104: <BaseLayout
105:   title="Dark Souls CRUD Web Service | Jared Street"
106:   description="PHP/MySQL CRUD web service with JavaScript AJAX interactions and JSON API responses."
107: >
108:   <section class="page-hero project-hero fade-in">
109:     <p class="eyebrow">PHP / MySQL / AJAX</p>
110:     <h1>Dark Souls CRUD Web Service</h1>
111:     <p>
112:       A themed PHP/MySQL CRUD web service where a browser client communicates
113:       with PHP API endpoints to create, read, update, and delete database
114:       records.
115:     </p>
116: 
117:     <div class="tech-list">
118:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
119:     </div>
120: 
121:     <div class="button-row">
122:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
123:     </div>
124:   </section>
125: 
126:   <section class="section-card project-section fade-in">
127:     <p class="eyebrow">Overview</p>
128:     <h2>Project Purpose</h2>
129:     <p>
130:       The Dark Souls CRUD Web Service demonstrates a full client-provider web
131:       service pattern. The provider side contains the PHP API, object classes,
132:       database class, SQL export, and tester page.
133:     </p>
134:     <p>
135:       The client side contains the HTML interface, JavaScript AJAX logic, CSS
136:       styling, sound effects, and particle animation used to create a themed user
137:       experience while still practicing practical CRUD service behavior.
138:     </p>
139:   </section>
140: 
141:   <section class="section-card project-section fade-in">
142:     <p class="eyebrow">Features</p>
143:     <h2>What the Application Does</h2>
144: 
145:     <ul class="feature-list">
146:       {features.map((feature) => <li>{feature}</li>)}
147:     </ul>
148:   </section>
149: 
150:   <section class="section-card project-section fade-in">
151:     <p class="eyebrow">Code Sample</p>
152:     <h2>Main API Controller Pattern</h2>
153:     <p>
154:       This sample shows the main API pattern: receive an action and table value,
155:       call the matching database method, and return a JSON response to the
156:       browser client.
157:     </p>
158: 
159:     <Code code={crudCode} lang="php" theme="github-dark" wrap />
160:   </section>
161: 
162:   <section class="section-card project-section fade-in">
163:     <p class="eyebrow">Screenshots</p>
164:     <h2>Application Screens</h2>
165: 
166:     <div class="screenshot-grid">
167:       {screenshots.map((screenshot) => (
168:         <figure class="screenshot-card">
169:           <img src={screenshot.src} alt={screenshot.alt} />
170:           <figcaption>
171:             <strong>{screenshot.title}</strong>
172:             <span>{screenshot.caption}</span>
173:           </figcaption>
174:         </figure>
175:       ))}
176:     </div>
177:   </section>
178: </BaseLayout>
````

## File: src/pages/projects/display-switcher.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const techStack = [
  6:   "Go",
  7:   "Cobra",
  8:   "JSON",
  9:   "Windows",
 10:   "MultiMonitorTool",
 11:   "CLI Automation",
 12: ];
 13: 
 14: const features = [
 15:   "Command-line interface for switching Windows display and workspace profiles",
 16:   "Cobra subcommands for organizing CLI behavior",
 17:   "JSON configuration file for named profiles",
 18:   "Global --config flag for custom config file paths",
 19:   "list command for showing available profiles",
 20:   "show command for inspecting profile actions",
 21:   "apply command for executing a selected profile",
 22:   "--dry-run flag for previewing actions without running them",
 23:   "Saved monitor layouts loaded through NirSoft MultiMonitorTool",
 24:   "Display-disabling actions for simplified monitor setups",
 25:   "Desktop application launching as part of workspace profiles",
 26:   "URL opening through the default browser",
 27:   "Separate profiles for bed, desk, school, and gaming workflows",
 28: ];
 29: 
 30: const screenshots = [
 31:   {
 32:     src: "/screenshots/display-switcher-list.png",
 33:     alt: "Display Switcher list command output",
 34:     title: "List Command",
 35:     caption: "Displays available workspace and monitor profiles.",
 36:   },
 37:   {
 38:     src: "/screenshots/display-switcher-show.png",
 39:     alt: "Display Switcher show command output",
 40:     title: "Show Command",
 41:     caption: "Displays the actions assigned to a selected profile.",
 42:   },
 43:   {
 44:     src: "/screenshots/display-switcher-apply.png",
 45:     alt: "Display Switcher apply command output",
 46:     title: "Apply Command",
 47:     caption:
 48:       "Applies a selected display profile and runs the configured workflow actions.",
 49:   },
 50: ];
 51: 
 52: const configCode = `type Config struct {
 53:     Profiles map[string]Profile \`json:"profiles"\`
 54: }
 55: 
 56: type Profile struct {
 57:     Actions []Action \`json:"actions"\`
 58: }
 59: 
 60: type Action struct {
 61:     Type string \`json:"type"\`
 62:     Path string \`json:"path,omitempty"\`
 63: }
 64: 
 65: func Load(path string) (Config, error) {
 66:     b, err := os.ReadFile(path)
 67:     if err != nil {
 68:         return Config{}, fmt.Errorf("read %q: %w", path, err)
 69:     }
 70: 
 71:     var cfg Config
 72:     if err := json.Unmarshal(b, &cfg); err != nil {
 73:         return Config{}, fmt.Errorf("parse %q: %w", path, err)
 74:     }
 75: 
 76:     return cfg, nil
 77: }`;
 78: ---
 79: 
 80: <BaseLayout
 81:   title="Display Switcher CLI | Jared Street"
 82:   description="Go command-line tool for switching Windows display profiles and launching workflow-specific applications."
 83: >
 84:   <section class="page-hero project-hero fade-in">
 85:     <p class="eyebrow">Go / CLI Tool</p>
 86:     <h1>Display Switcher CLI</h1>
 87:     <p>
 88:       A Go command-line application for switching between Windows monitor and
 89:       workspace setups. The tool reads named profiles from JSON and applies
 90:       actions such as loading monitor layouts, disabling displays, launching
 91:       apps, and opening URLs.
 92:     </p>
 93: 
 94:     <div class="tech-list">
 95:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
 96:     </div>
 97: 
 98:     <div class="button-row">
 99:       <a
100:         class="button button-primary"
101:         href="https://stc.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=0107982d-c1fc-4c68-8597-b40701357aba"
102:         target="_blank"
103:         rel="noopener noreferrer"
104:       >
105:         View Live Demo
106:       </a>
107:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
108:     </div>
109:   </section>
110: 
111:   <section class="section-card project-section fade-in">
112:     <p class="eyebrow">Overview</p>
113:     <h2>Project Purpose</h2>
114:     <p>
115:       Display Switcher CLI was built as a practical automation tool for managing
116:       different computer setups. One profile can restore a full desk layout with
117:       multiple monitors, while another can simplify the display setup for use
118:       from bed.
119:     </p>
120:     <p>
121:       The project also supports workflow automation beyond monitor layout. A
122:       profile can launch school-related applications, gaming tools, or useful
123:       websites after the display configuration is applied.
124:     </p>
125:   </section>
126: 
127:   <section class="section-card project-section fade-in">
128:     <p class="eyebrow">Features</p>
129:     <h2>What the Tool Does</h2>
130: 
131:     <ul class="feature-list">
132:       {features.map((feature) => <li>{feature}</li>)}
133:     </ul>
134:   </section>
135: 
136:   <section class="section-card project-section fade-in">
137:     <p class="eyebrow">Code Sample</p>
138:     <h2>Loading Profile Configuration</h2>
139:     <p>
140:       This sample shows the configuration-loading logic. The CLI reads a JSON
141:       file, parses it into Go structs, and returns a usable configuration object
142:       to the command files.
143:     </p>
144: 
145:     <Code code={configCode} lang="go" theme="github-dark" wrap />
146:   </section>
147: 
148:   <section class="section-card project-section fade-in">
149:     <p class="eyebrow">Screenshots</p>
150:     <h2>CLI Output</h2>
151: 
152:     <div class="screenshot-grid">
153:       {screenshots.map((screenshot) => (
154:         <figure class="screenshot-card">
155:           <img src={screenshot.src} alt={screenshot.alt} />
156:           <figcaption>
157:             <strong>{screenshot.title}</strong>
158:             <span>{screenshot.caption}</span>
159:           </figcaption>
160:         </figure>
161:       ))}
162:     </div>
163:   </section>
164: 
165: 
166: </BaseLayout>
````

## File: src/pages/projects/godot-roguelike.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const techStack = [
  6:   "Godot 4.4.1",
  7:   "C#",
  8:   ".NET",
  9:   "TileMapLayer",
 10:   "Node2D",
 11:   "Game Systems",
 12: ];
 13: 
 14: const features = [
 15:   "Turn-based grid movement using keyboard input",
 16:   "Tile-based collision and walkability checks",
 17:   "Player bump-attacks when moving into an occupied enemy tile",
 18:   "Sequential enemy turn resolution after the player acts",
 19:   "Enemy movement and adjacency-based attacks",
 20:   "Multiple combat floors with a final boss floor",
 21:   "Reward selection between non-boss floors",
 22:   "Persistent run state across scene changes",
 23:   "Player stats for health, max health, damage, enemies defeated, and total damage dealt",
 24:   "Active abilities including Whirlwind, Attack Buff, and Heal",
 25:   "Passive reward effects such as healing on kill, regeneration, and scaling damage bonuses",
 26:   "Gear rewards such as Iron Charm and Rage Mask",
 27:   "Combat log using styled RichTextLabel text",
 28:   "Start menu, reward screen, game over screen, and victory screen",
 29: ];
 30: 
 31: const screenshots = [
 32:   {
 33:     src: "/screenshots/roguelike-start-menu.png",
 34:     alt: "Godot roguelike start menu",
 35:     title: "Start Menu",
 36:     caption: "Start menu used to begin a new run.",
 37:   },
 38:   {
 39:     src: "/screenshots/roguelike-combat-floor.png",
 40:     alt: "Godot roguelike combat floor with player and enemies",
 41:     title: "Combat Floor",
 42:     caption:
 43:       "Grid-based combat floor with player movement, enemies, UI, and combat log.",
 44:   },
 45:   {
 46:     src: "/screenshots/roguelike-reward-selection.png",
 47:     alt: "Godot roguelike reward selection screen",
 48:     title: "Reward Selection",
 49:     caption:
 50:       "Reward cards presented between floors to improve the current run.",
 51:   },
 52:   {
 53:     src: "/screenshots/roguelike-final-floor.png",
 54:     alt: "Godot roguelike final floor",
 55:     title: "Final Floor",
 56:     caption: "Final combat floor before the end-screen flow.",
 57:   },
 58:   {
 59:     src: "/screenshots/roguelike-end-screen.png",
 60:     alt: "Godot roguelike end screen",
 61:     title: "End Screen",
 62:     caption: "Victory or game-over flow after the run ends.",
 63:   },
 64: ];
 65: 
 66: const runEffectsCode = `public static class RunEffects
 67: {
 68:     public static int GetEffectiveMaxHealth(Player player, RunState runState)
 69:     {
 70:         int maxHealth = runState.BaseMaxHealth;
 71: 
 72:         if (runState.CurrentGear == RunState.GearType.IronCharm)
 73:             maxHealth += 15;
 74: 
 75:         return maxHealth;
 76:     }
 77: 
 78:     public static int GetEffectiveDamage(Player player, RunState runState)
 79:     {
 80:         int damage = runState.BaseDamage;
 81: 
 82:         if (runState.CurrentGear == RunState.GearType.RageMask &&
 83:             player.Health * 2 < GetEffectiveMaxHealth(player, runState))
 84:         {
 85:             damage += 2;
 86:         }
 87: 
 88:         if (player.NextAttackBuffed)
 89:         {
 90:             damage *= 2;
 91:         }
 92: 
 93:         return damage;
 94:     }
 95: 
 96:     public static void OnEnemyKilled(Player player, RunState runState, Start map)
 97:     {
 98:         if (runState.OwnedBoons.Contains(RunState.BoonType.HealOnKill))
 99:         {
100:             player.Health = Math.Min(
101:                 player.Health + 1,
102:                 GetEffectiveMaxHealth(player, runState)
103:             );
104: 
105:             map.AddLogMessageRaw(
106:                 $"[color=green]Life Tap[/color] restores [color=green]1 HP[/color]."
107:             );
108:         }
109: 
110:         if (runState.OwnedBoons.Contains(RunState.BoonType.CrushingWeight))
111:         {
112:             int newTier = runState.EnemiesDefeated / 5;
113: 
114:             if (newTier > runState.CrushingWeightTiersAwarded)
115:             {
116:                 int tiersGained = newTier - runState.CrushingWeightTiersAwarded;
117:                 runState.BaseDamage += tiersGained;
118:                 runState.CrushingWeightTiersAwarded = newTier;
119: 
120:                 map.AddLogMessageRaw(
121:                     $"[color=orange]Crushing Weight[/color] grants " +
122:                     $"[color=yellow]+{tiersGained} damage[/color]."
123:                 );
124:             }
125:         }
126: 
127:         SyncPlayerStats(player, runState);
128:     }
129: }`;
130: ---
131: 
132: <BaseLayout
133:   title="Godot Grid Roguelike | Jared Street"
134:   description="Turn-based Godot roguelike prototype with grid movement, combat, rewards, abilities, and persistent run state."
135: >
136:   <section class="page-hero project-hero fade-in">
137:     <p class="eyebrow">Game Systems / C#</p>
138:     <h1>Godot Grid Roguelike Prototype</h1>
139:     <p>
140:       A turn-based dungeon crawler built in Godot 4.4.1 with C#. The project
141:       focuses on grid-based movement, combat turns, reward selection, player
142:       abilities, and persistent run progression.
143:     </p>
144: 
145:     <div class="tech-list">
146:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
147:     </div>
148: 
149:     <div class="button-row">
150:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
151:     </div>
152:   </section>
153: 
154:   <section class="section-card project-section fade-in">
155:     <p class="eyebrow">Overview</p>
156:     <h2>Project Purpose</h2>
157:     <p>
158:       The Godot Grid Roguelike Prototype is a small but complete gameplay loop:
159:       the player starts a run, moves through tile-based combat floors, defeats
160:       enemies, selects rewards, and continues until victory or game over.
161:     </p>
162:     <p>
163:       The main development challenge was coordinating turn order and state. The
164:       player acts first, then enemies resolve their turns, while health, damage,
165:       rewards, boons, gear, and floor progress persist across scene changes.
166:     </p>
167:   </section>
168: 
169:   <section class="section-card project-section fade-in">
170:     <p class="eyebrow">Features</p>
171:     <h2>What the Prototype Includes</h2>
172: 
173:     <ul class="feature-list">
174:       {features.map((feature) => <li>{feature}</li>)}
175:     </ul>
176:   </section>
177: 
178:   <section class="section-card project-section fade-in">
179:     <p class="eyebrow">Code Sample</p>
180:     <h2>Reward and Gear Effect Logic</h2>
181:     <p>
182:       This sample shows how the project calculates derived combat stats and
183:       applies persistent reward effects. Gear and boons are not just displayed in
184:       the UI; they directly affect damage, healing, and long-term run scaling.
185:     </p>
186: 
187:     <Code code={runEffectsCode} lang="csharp" theme="github-dark" wrap />
188:   </section>
189: 
190:   <section class="section-card project-section fade-in">
191:     <p class="eyebrow">Screenshots</p>
192:     <h2>Application Screens</h2>
193: 
194:     <div class="screenshot-grid">
195:       {screenshots.map((screenshot) => (
196:         <figure class="screenshot-card">
197:           <img src={screenshot.src} alt={screenshot.alt} />
198:           <figcaption>
199:             <strong>{screenshot.title}</strong>
200:             <span>{screenshot.caption}</span>
201:           </figcaption>
202:         </figure>
203:       ))}
204:     </div>
205:   </section>
206: </BaseLayout>
````

## File: src/pages/projects/index.astro
````astro
  1: ---
  2: import { Image } from "astro:assets";
  3: import BaseLayout from "../../layouts/BaseLayout.astro";
  4: 
  5: const projectCategories = [
  6:   {
  7:     name: "C# / .NET",
  8:     description: "Application and service projects built with C#, ASP.NET Core, MVC, Entity Framework, and WCF.",
  9:     projects: [
 10:       {
 11:         title: "SportsPro Technical Support",
 12:         href: "/projects/sportspro/",
 13:         summary: "ASP.NET Core MVC support management system with database-backed CRUD workflows.",
 14:         tech: ["C#", "ASP.NET Core MVC", "Entity Framework", "SQL Server"],
 15:         image: "/screenshots/sportspro-home.png",
 16:         imageAlt: "SportsPro Technical Support home page",
 17:       },
 18:       {
 19:         title: "WCF Service Project",
 20:         href: "/projects/wcf/",
 21:         summary: "Service/client project demonstrating C# service methods and structured communication.",
 22:         tech: ["C#", "WCF", ".NET Framework", "SOAP"],
 23:         image: "/screenshots/library-wcf-service-browser.png",
 24:         imageAlt: "Library WCF service running in browser",
 25:       },
 26:     ],
 27:   },
 28:   {
 29:     name: "PHP / MySQL",
 30:     description: "Database-backed web applications and REST-style services built with PHP, MySQL, JSON, and AJAX.",
 31:     projects: [
 32:       {
 33:         title: "Simple Forum Application",
 34:         href: "/projects/simple-forum/",
 35:         summary: "Dynamic forum application with users, posts, categories, sessions, and database persistence.",
 36:         tech: ["PHP", "MySQL", "PDO", "Sessions"],
 37:         image: "/screenshots/simple-forum-home.png",
 38:         imageAlt: "Simple Forum home page",
 39:       },
 40:       {
 41:         title: "RESTful Student Contacts Service",
 42:         href: "/projects/rest-ajax-php/",
 43:         summary: "PHP/MySQL service that returns JSON data and is consumed by an AJAX client.",
 44:         tech: ["PHP", "MySQL", "AJAX", "JSON"],
 45:         image: "/screenshots/RESTful-AJAX-home.png",
 46:         imageAlt: "RESTful Student Contacts Service home page",
 47:       },
 48:       {
 49:         title: "Dark Souls CRUD Web Service",
 50:         href: "/projects/crud-restful-service/",
 51:         summary: "Themed CRUD web service with PHP API endpoints, MySQL tables, and AJAX interactions.",
 52:         tech: ["PHP", "MySQL", "JavaScript", "jQuery AJAX"],
 53:         image: "/screenshots/darksouls-home.png",
 54:         imageAlt: "Dark Souls CRUD web service home page",
 55:       },
 56:     ],
 57:   },
 58:   {
 59:     name: "Go / CLI Tools",
 60:     description: "Command-line tools and automation projects focused on practical desktop workflows.",
 61:     projects: [
 62:       {
 63:         title: "Display Switching CLI",
 64:         href: "/projects/display-switcher/",
 65:         summary: "Go command-line tool for switching Windows display profiles and launching workflow-specific apps.",
 66:         tech: ["Go", "Cobra", "JSON", "Windows"],
 67:         image: "/screenshots/display-switcher-show.png",
 68:         imageAlt: "Display Switcher CLI home page",
 69:       },
 70:     ],
 71:   },
 72:   {
 73:     name: "Game / C#",
 74:     description: "Gameplay prototypes and interactive systems built with C# outside of traditional business applications.",
 75:     projects: [
 76:       {
 77:         title: "Godot Grid Roguelike Prototype",
 78:         href: "/projects/godot-roguelike/",
 79:         summary: "Turn-based grid roguelike prototype with combat, enemy turns, rewards, and persistent run state.",
 80:         tech: ["Godot", "C#", "Game Systems", "Tilemaps"],
 81:         image: "/screenshots/roguelike-combat-floor.png",
 82:         imageAlt: "Godot Grid Roguelike Prototype home page",
 83:       },
 84:       {
 85:         title: "Troll Pong Gamejam Entry",
 86:         summary: "A game jam I participated in with 2 other people using mob programming methods. The theme of the game jam was WarioWare.",
 87:         href: "https://severalherr.itch.io/troll-pong",
 88:         Image: "/screenshots/troll-pong.png",
 89:         imageAlt: "Troll Pong gamejam entry",
 90:         tech: ["Godot", "C#", "Game Systems"],
 91:       }
 92:     ],
 93:   },
 94:   {
 95:     name: "JavaScript / Realtime",
 96:     description: "Client-side and realtime projects using JavaScript and event-driven web behavior.",
 97:     projects: [
 98:     {
 99:       title: "Realtime Voting System",
100:       href: "/projects/voting-system/",
101:       summary: "Realtime voting demo using browser-based interaction and live result updates.",
102:       tech: ["JavaScript", "Node.js", "Socket.IO", "HTML/CSS"],
103:       image: "/screenshots/realtime-voting-home.png",
104:       imageAlt: "Realtime voting application page",
105:     },
106:     ],
107:   },
108: ];
109: 
110: const courseworkArchive = {
111:   title: "Coursework & Syllabi Archive",
112:   href: "/coursework/",
113:   summary:
114:     "An archive of CIS course syllabi and academic materials from Southeast Technical College.",
115: };
116: ---
117: 
118: <BaseLayout
119:   title="Projects | Jared Street"
120:   description="Project library for Jared Street, organized by technology area and project type."
121: >
122:   <section class="page-hero fade-in">
123:     <p class="eyebrow">Project Library</p>
124:     <h1>Projects</h1>
125:     <p>
126:       A collection of web, database, application, service, CLI, and game projects.
127:     </p>
128:   </section>
129: 
130:   <section class="project-library fade-in" aria-labelledby="project-library-heading">
131:     <div class="section-heading">
132:       <p class="eyebrow">Browse by Category</p>
133:       <h2 id="project-library-heading">Explore Project Areas</h2>
134:       <p>
135:         Open a category to view related projects and jump to individual project documentation.
136:       </p>
137:     </div>
138: 
139:     <div class="category-grid">
140:       {projectCategories.map((category) => (
141:         <article class="category-card hover-category-card">
142:           <div class="category-card-header">
143:             <span>
144:               <strong>{category.name}</strong>
145:               <small>
146:                 {category.projects.length} project{category.projects.length === 1 ? "" : "s"}
147:               </small>
148:             </span>
149:           </div>
150: 
151:           <div class="category-card-body">
152:             <p>{category.description}</p>
153: 
154:           <div class="category-carousel" data-carousel>
155:             {category.projects.length > 1 && (
156:               <div class="carousel-controls">
157:                 <button
158:                   class="carousel-button"
159:                   type="button"
160:                   data-carousel-prev
161:                   aria-label={`View previous ${category.name} project`}
162:                 >
163:                   ←
164:                 </button>
165: 
166:                 <span class="carousel-count">
167:                   <span data-carousel-index>1</span> / {category.projects.length}
168:                 </span>
169: 
170:                 <button
171:                   class="carousel-button"
172:                   type="button"
173:                   data-carousel-next
174:                   aria-label={`View next ${category.name} project`}
175:                 >
176:                   →
177:                 </button>
178:               </div>
179:             )}
180: 
181:             <div class="category-project-window">
182:               {category.projects.map((project, index) => (
183:                 <article
184:                   class={`project-slide ${index === 0 ? "is-active" : ""}`}
185:                   data-carousel-slide
186:                 >
187:                   {project.image ? (
188:                     <img
189:                       class="project-slide-image"
190:                       src={project.image}
191:                       alt={project.imageAlt}
192:                     />
193:                   ) : (
194:                     <div class="project-image-placeholder">
195:                       Project documentation
196:                     </div>
197:                   )}
198: 
199:                   <div class="project-slide-content">
200:                     <h3>
201:                       <a href={project.href}>{project.title}</a>
202:                     </h3>
203: 
204:                     <p>{project.summary}</p>
205: 
206:                     <div class="tech-list">
207:                       {project.tech.map((techItem) => (
208:                         <span class="tech-pill">{techItem}</span>
209:                       ))}
210:                     </div>
211: 
212:                     <a class="text-link" href={project.href}>
213:                       View Project
214:                     </a>
215:                   </div>
216:                 </article>
217:               ))}
218:             </div>
219:           </div>
220:           </div>
221:         </article>
222:       ))}
223:     </div>
224:   </section>
225: 
226:   <section class="section-card coursework-callout fade-in" aria-labelledby="coursework-archive-heading">
227:     <div>
228:       <p class="eyebrow">Supporting Materials</p>
229:       <h2 id="coursework-archive-heading">{courseworkArchive.title}</h2>
230:       <p>{courseworkArchive.summary}</p>
231:     </div>
232: 
233:     <div class="coursework-callout-action">
234:       <a class="button button-secondary" href={courseworkArchive.href}>
235:         View Coursework Archive
236:       </a>
237:     </div>
238: </section>
239: </BaseLayout>
240: <script>
241:   document.querySelectorAll("[data-carousel]").forEach((carousel) => {0
242:     const slides = Array.from(
243:       carousel.querySelectorAll("[data-carousel-slide]")
244:     );
245: 
246:     const previousButton = carousel.querySelector("[data-carousel-prev]");
247:     const nextButton = carousel.querySelector("[data-carousel-next]");
248:     const indexLabel = carousel.querySelector("[data-carousel-index]");
249: 
250:     if (slides.length === 0) return;
251: 
252:     let currentIndex = 0;
253: 
254:     function showSlide(nextIndex: number) {
255:       currentIndex = (nextIndex + slides.length) % slides.length;
256: 
257:       slides.forEach((slide, index) => {
258:         slide.classList.toggle("is-active", index === currentIndex);
259:       });
260: 
261:       if (indexLabel) {
262:         indexLabel.textContent = String(currentIndex + 1);
263:       }
264:     }
265: 
266:     previousButton?.addEventListener("click", () => {
267:       showSlide(currentIndex - 1);
268:     });
269: 
270:     nextButton?.addEventListener("click", () => {
271:       showSlide(currentIndex + 1);
272:     });
273: 
274:     showSlide(0);
275:   });
276: </script>
````

## File: src/pages/projects/rest-ajax-php.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const restAjaxCode = `<?php
  6: include_once("class_lib/StrJDB_Access.php");
  7: 
  8: $DB_Access = new StrJDB_Access();
  9: $table = "strj_unit2_ex1_contacts";
 10: 
 11: $contact_id = $_GET['contact_id'] ?? "";
 12: 
 13: if ($contact_id === "") {
 14:     print(json_encode(array("error" => "contact_id parameter is required")));
 15:     exit;
 16: }
 17: 
 18: $DB_Result = $DB_Access->selectOne($table, $contact_id);
 19: 
 20: if ($DB_Result && $row = $DB_Result->fetch_assoc()) {
 21:     print(json_encode($row));
 22: } else {
 23:     print(json_encode(array("error" => "Record not found")));
 24: }
 25: ?>`;
 26: 
 27: const techStack = [
 28:   "PHP",
 29:   "MySQL",
 30:   "JSON",
 31:   "AJAX",
 32:   "jQuery",
 33:   "JavaScript",
 34:   "HTML",
 35:   "CSS",
 36: ];
 37: 
 38: const features = [
 39:   "Connects to a MySQL database named students",
 40:   "Uses a reusable PHP database access class for database operations",
 41:   "Displays all contact records from the student contacts table",
 42:   "Retrieves a single contact record by contact_id",
 43:   "Returns API responses as JSON using json_encode()",
 44:   "Includes API tester pages for directly checking service output",
 45:   "Includes client pages that consume the APIs with jQuery AJAX requests",
 46:   "Displays returned JSON data dynamically in the browser",
 47:   "Handles missing or invalid contact IDs with JSON error messages",
 48:   "Includes a SQL script for creating and populating the contacts table",
 49: ];
 50: 
 51: const screenshots = [
 52:   {
 53:     src: "/screenshots/RESTful-AJAX-home.png",
 54:     alt: "RESTful Student Contacts project home page",
 55:     title: "Home / Project Links Page",
 56:     caption: "Main project page linking to the client and service test pages.",
 57:   },
 58:   {
 59:     src: "/screenshots/RESTful-AJAX-display-all.png",
 60:     alt: "Display all student contact records client page",
 61:     title: "Display All Records Client",
 62:     caption: "AJAX client page displaying all records returned by the PHP service.",
 63:   },
 64:   {
 65:     src: "/screenshots/RESTful-AJAX-display-one.png",
 66:     alt: "Display one student contact record client page",
 67:     title: "Display One Record Client",
 68:     caption: "Client page retrieving one contact record by contact ID.",
 69:   },
 70: ];
 71: ---
 72: 
 73: <BaseLayout
 74:   title="RESTful Student Contacts Service | Jared Street"
 75:   description="PHP/MySQL REST-style service returning JSON data to AJAX client pages."
 76: >
 77:   <section class="page-hero project-hero fade-in">
 78:     <p class="eyebrow">PHP / MySQL / AJAX</p>
 79:     <h1>RESTful Student Contacts Service</h1>
 80:     <p>
 81:       A PHP/MySQL web service project that retrieves student contact records,
 82:       encodes them as JSON, and exposes the data to browser-based client pages
 83:       through REST-style endpoints.
 84:     </p>
 85: 
 86:     <div class="tech-list">
 87:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
 88:     </div>
 89: 
 90:     <div class="button-row">
 91:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
 92:     </div>
 93:   </section>
 94: 
 95:   <section class="section-card project-section fade-in">
 96:     <p class="eyebrow">Overview</p>
 97:     <h2>Project Purpose</h2>
 98:     <p>
 99:       The RESTful Student Contacts Service demonstrates how a server-side PHP
100:       application can connect to a MySQL database, retrieve records, encode the
101:       results as JSON, and return that data to client-side pages.
102:     </p>
103:     <p>
104:       The application separates provider files from client files. The provider
105:       side handles database access and JSON output, while the client side uses
106:       jQuery AJAX requests to display all records or retrieve a selected record
107:       by contact ID.
108:     </p>
109:   </section>
110: 
111:   <section class="section-card project-section fade-in">
112:     <p class="eyebrow">Features</p>
113:     <h2>What the Service Does</h2>
114: 
115:     <ul class="feature-list">
116:       {features.map((feature) => <li>{feature}</li>)}
117:     </ul>
118:   </section>
119: 
120:   <section class="section-card project-section fade-in">
121:     <p class="eyebrow">Code Sample</p>
122:     <h2>Returning One Contact as JSON</h2>
123:     <p>
124:       This PHP endpoint reads a contact ID from the query string, validates that
125:       it was provided, calls the database access class, and returns either the
126:       matching record or an error message as JSON.
127:     </p>
128: 
129:     <Code code={restAjaxCode} lang="php" theme="github-dark" wrap />
130:   </section>
131: 
132:   <section class="section-card project-section fade-in">
133:     <p class="eyebrow">Screenshots</p>
134:     <h2>Application Screens</h2>
135: 
136:     <div class="screenshot-grid">
137:       {screenshots.map((screenshot) => (
138:         <figure class="screenshot-card">
139:           <img src={screenshot.src} alt={screenshot.alt} />
140:           <figcaption>
141:             <strong>{screenshot.title}</strong>
142:             <span>{screenshot.caption}</span>
143:           </figcaption>
144:         </figure>
145:       ))}
146:     </div>
147:   </section>
148: </BaseLayout>
````

## File: src/pages/projects/simple-forum.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const simpleForumCode = `function update_post($id, $title, $content) {
  6:     global $db;
  7: 
  8:     $query = 'UPDATE posts
  9:               SET title = :title,
 10:                   content = :content
 11:               WHERE id = :id';
 12: 
 13:     $statement = $db->prepare($query);
 14:     $statement->bindValue(':title', $title);
 15:     $statement->bindValue(':content', $content);
 16:     $statement->bindValue(':id', $id, PDO::PARAM_INT);
 17: 
 18:     $success = $statement->execute();
 19:     $statement->closeCursor();
 20: 
 21:     return $success;
 22: }`;
 23: 
 24: const techStack = [
 25:   "PHP",
 26:   "MySQL",
 27:   "PDO",
 28:   "Sessions",
 29:   "Password Hashing",
 30:   "Bootstrap",
 31: ];
 32: 
 33: const features = [
 34:   "User registration with username, email, and password fields",
 35:   "Secure password hashing using PHP password_hash()",
 36:   "Login validation using password_verify()",
 37:   "Session-based login and logout functionality",
 38:   "Optional Remember Me token stored in the database",
 39:   "Forum categories loaded from MySQL",
 40:   "Category-based post browsing",
 41:   "Create, edit, and delete forum posts",
 42:   "PDO prepared statements for database queries",
 43:   "Responsive Bootstrap layout",
 44:   "Navigation that changes based on login state",
 45: ];
 46: 
 47: const screenshots = [
 48:   {
 49:     src: "/screenshots/simple-forum-home.png",
 50:     alt: "Simple Forum home page showing forum categories",
 51:     title: "Forum Categories",
 52:     caption: "Forum categories loaded dynamically from the database.",
 53:   },
 54:   {
 55:     src: "/screenshots/simple-forum-create-post.png",
 56:     alt: "Simple Forum create post page",
 57:     title: "Create Post",
 58:     caption: "Authenticated users can create new forum posts.",
 59:   },
 60:   {
 61:     src: "/screenshots/simple-forum-view-post.png",
 62:     alt: "Simple Forum posts page",
 63:     title: "Viewing Posts",
 64:     caption: "Posts displayed for a selected forum category.",
 65:   },
 66: ];
 67: ---
 68: 
 69: <BaseLayout
 70:   title="Simple Forum Application | Jared Street"
 71:   description="PHP and MySQL forum application with authentication, sessions, posts, categories, and database persistence."
 72: >
 73:   <section class="page-hero project-hero fade-in">
 74:     <p class="eyebrow">PHP / MySQL</p>
 75:     <h1>Simple Forum Application</h1>
 76:     <p>
 77:       A dynamic forum application where users can register, log in, browse
 78:       categories, create posts, edit posts, and delete posts using a MySQL-backed
 79:       PHP application.
 80:     </p>
 81: 
 82:     <div class="tech-list">
 83:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
 84:     </div>
 85: 
 86:     <div class="button-row">
 87:       <a
 88:         class="button button-primary"
 89:         href="https://cis241simpleforum.ct.ws/index.php"
 90:         target="_blank"
 91:         rel="noopener noreferrer"
 92:       >
 93:         View Live Demo
 94:       </a>
 95:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
 96:     </div>
 97:   </section>
 98: 
 99:   <section class="section-card project-section fade-in">
100:     <p class="eyebrow ">Overview</p>
101:     <h2>Project Purpose</h2>
102:     <p>
103:       The Simple Forum Application is a PHP/MySQL web application focused on
104:       database-backed user interaction. It includes account creation, login,
105:       session handling, forum categories, and post management.
106:     </p>
107:     <p>
108:       The project demonstrates server-side web development using PHP, relational
109:       database tables, prepared SQL statements, authentication checks, and
110:       dynamic pages that change based on whether the user is logged in.
111:     </p>
112:   </section>
113: 
114:   <section class="section-card project-section fade-in">
115:     <p class="eyebrow">Features</p>
116:     <h2>What the Application Does</h2>
117: 
118:     <ul class="feature-list">
119:       {features.map((feature) => <li>{feature}</li>)}
120:     </ul>
121:   </section>
122: 
123:   <section class="section-card project-section fade-in">
124:     <p class="eyebrow">Code Sample</p>
125:     <h2>Updating Posts with a Prepared Statement</h2>
126:     <p>
127:       This function updates a forum post using a prepared SQL statement. User
128:       values are bound to named parameters before the query executes.
129:     </p>
130: 
131:     <Code code={simpleForumCode} lang="php" theme="github-dark" wrap />
132: 
133:     <p>
134:       This is the main database-access pattern used throughout the project:
135:       prepare the SQL query, bind user-provided values, execute the statement,
136:       and close the cursor.
137:     </p>
138:   </section>
139: 
140:   <section class="section-card project-section fade-in">
141:     <p class="eyebrow">Screenshots</p>
142:     <h2>Application Screens</h2>
143: 
144:     <div class="screenshot-grid">
145:       {screenshots.map((screenshot) => (
146:         <figure class="screenshot-card">
147:           <img src={screenshot.src} alt={screenshot.alt} />
148:           <figcaption>
149:             <strong>{screenshot.title}</strong>
150:             <span>{screenshot.caption}</span>
151:           </figcaption>
152:         </figure>
153:       ))}
154:     </div>
155:   </section>
156: </BaseLayout>
````

## File: src/pages/projects/sportspro.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const sportsProCode = `[HttpGet]
  6: [Route("Incidents")]
  7: public ViewResult List(IncidentListViewModel model)
  8: {
  9:     IQueryable<Incident> query = context.Incidents
 10:         .Include(i => i.Customer)
 11:         .Include(i => i.Product)
 12:         .Include(i => i.Technician);
 13: 
 14:     if (model.IncidentStatus == "unassigned")
 15:     {
 16:         query = query.Where(i => i.TechnicianID == -1);
 17:     }
 18:     else if (model.IncidentStatus == "open")
 19:     {
 20:         query = query.Where(i => i.DateClosed == null);
 21:     }
 22: 
 23:     model.Incidents = query.OrderBy(i => i.DateOpened).ToList();
 24: 
 25:     return View(model);
 26: }`;
 27: 
 28: const techStack = [
 29:   "C#",
 30:   "ASP.NET Core MVC",
 31:   "Entity Framework Core",
 32:   "SQL Server",
 33:   "Razor Views",
 34:   "Bootstrap",
 35: ];
 36: 
 37: const features = [
 38:   "Product, customer, technician, and incident management",
 39:   "List, add, edit, and delete workflows using MVC controllers and Razor views",
 40:   "Incident filtering by status, including open and unassigned incidents",
 41:   "Entity Framework Core database access with related customer, product, and technician data",
 42:   "View models used to pass filtered data into Razor views",
 43:   "Server-side validation for required fields, string lengths, ranges, and dates",
 44:   "Initial database migration and seed data for core support records",
 45:   "Bootstrap-based layout for consistent page structure",
 46: ];
 47: 
 48: const screenshots = [
 49:   {
 50:     src: "/screenshots/sportspro-home.png",
 51:     alt: "SportsPro home page",
 52:     title: "Home Page",
 53:     caption: "Landing page for the SportsPro technical support application.",
 54:   },
 55:   {
 56:     src: "/screenshots/sportspro-incidents.png",
 57:     alt: "SportsPro incident list with filters",
 58:     title: "Incident List and Filters",
 59:     caption:
 60:       "Incident list showing related customer, product, technician, and status information.",
 61:   },
 62:   {
 63:     src: "/screenshots/sportspro-technician-incidents.png",
 64:     alt: "SportsPro technician incident workflow",
 65:     title: "Technician Incident Workflow",
 66:     caption:
 67:       "Technician-specific workflow for selecting a technician and updating assigned incidents.",
 68:   },
 69: ];
 70: ---
 71: 
 72: <BaseLayout
 73:   title="SportsPro Technical Support | Jared Street"
 74:   description="ASP.NET Core MVC support management system with database-backed CRUD workflows."
 75: >
 76:   <section class="page-hero project-hero fade-in">
 77:     <p class="eyebrow">C# / ASP.NET Core</p>
 78:     <h1>SportsPro Technical Support</h1>
 79:     <p>
 80:       A database-backed ASP.NET Core MVC application for managing technical support
 81:       records, including products, customers, technicians, and incidents.
 82:     </p>
 83: 
 84:     <div class="tech-list">
 85:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
 86:     </div>
 87: 
 88:     <div class="button-row">
 89:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
 90:     </div>
 91:   </section>
 92: 
 93:   <section class="section-card project-section fade-in">
 94:     <p class="eyebrow">Overview</p>
 95:     <h2>Project Purpose</h2>
 96:     <p>
 97:       SportsPro Technical Support is an ASP.NET Core MVC application built around
 98:       a practical support-desk workflow. The system allows users to maintain
 99:       product, customer, technician, and incident records through standard
100:       database-backed CRUD operations.
101:     </p>
102:     <p>
103:       The project demonstrates core application-development patterns: MVC routing,
104:       controller actions, Razor views, Entity Framework Core queries, model
105:       validation, relational data, and view models used to organize page-specific
106:       data.
107:     </p>
108:   </section>
109: 
110:   <section class="section-card project-section fade-in">
111:     <p class="eyebrow">Features</p>
112:     <h2>What the Application Does</h2>
113: 
114:     <ul class="feature-list">
115:       {features.map((feature) => <li>{feature}</li>)}
116:     </ul>
117:   </section>
118: 
119:   <section class="section-card project-section fade-in">
120:     <p class="eyebrow">Code Sample</p>
121:     <h2>Filtering Incidents with Entity Framework</h2>
122:     <p>
123:       This controller action builds an Entity Framework query, includes related
124:       records needed by the view, applies filtering logic, and returns the
125:       populated view model to the Razor page.
126:     </p>
127: 
128:     <Code code={sportsProCode} lang="csharp" theme="github-dark" wrap />
129: 
130:     <p>
131:       The important pattern here is separation of responsibilities: the controller
132:       prepares the data, Entity Framework handles the database query, and the
133:       Razor view focuses on presentation.
134:     </p>
135:   </section>
136: 
137:   <section class="section-card project-section fade-in">
138:     <p class="eyebrow">Screenshots</p>
139:     <h2>Application Screens</h2>
140: 
141:     <div class="screenshot-grid">
142:       {screenshots.map((screenshot) => (
143:         <figure class="screenshot-card">
144:           <img src={screenshot.src} alt={screenshot.alt} />
145:           <figcaption>
146:             <strong>{screenshot.title}</strong>
147:             <span>{screenshot.caption}</span>
148:           </figcaption>
149:         </figure>
150:       ))}
151:     </div>
152:   </section>
153: </BaseLayout>
````

## File: src/pages/projects/voting-system.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const votingCode = `// Socket.IO setup
  6: const io = require('socket.io')(server, {
  7:     cors: { origin: '*' }
  8: });
  9: 
 10: // Voting state
 11: let votes = {
 12:     JavaScript: 0,
 13:     Python: 0,
 14:     'C#': 0
 15: };
 16: 
 17: // Handle socket connections
 18: io.on('connection', (socket) => {
 19:     console.log('User connected');
 20: 
 21:     // Send current results immediately
 22:     socket.emit('updateResults', votes);
 23: 
 24:     // Handle vote
 25:     socket.on('vote', (option) => {
 26:         if (votes[option] !== undefined) {
 27:             votes[option]++;
 28:             io.emit('updateResults', votes);
 29:         }
 30:     });
 31: 
 32:     // Reset poll
 33:     socket.on('reset', () => {
 34:         for (let key in votes) {
 35:             votes[key] = 0;
 36:         }
 37: 
 38:         io.emit('updateResults', votes);
 39:     });
 40: });`;
 41: 
 42: const techStack = [
 43:   "Node.js",
 44:   "Socket.IO",
 45:   "JavaScript",
 46:   "HTML",
 47:   "CSS",
 48:   "Realtime Events",
 49: ];
 50: 
 51: const features = [
 52:   "Allows users to vote for JavaScript, Python, or C#",
 53:   "Sends votes from the browser to the server using Socket.IO events",
 54:   "Stores live vote counts on the Node.js server",
 55:   "Broadcasts updated results to all connected clients",
 56:   "Updates the browser interface instantly without refreshing the page",
 57:   "Displays vote counts beside each poll option",
 58:   "Calculates result percentages based on the current vote total",
 59:   "Displays animated horizontal result bars",
 60:   "Includes a reset button that clears all vote totals",
 61:   "Supports testing with multiple browser tabs to simulate multiple users",
 62:   "Serves the client HTML, JavaScript, and CSS files from the Node.js server",
 63: ];
 64: 
 65: const screenshots = [
 66:   {
 67:     src: "/screenshots/realtime-voting-home.png",
 68:     alt: "Real-time voting application page",
 69:     title: "Voting Page with Multiple Clients",
 70:     caption: "Voting interface used by connected clients.",
 71:   },
 72:   {
 73:     src: "/screenshots/realtime-voting-results.png",
 74:     alt: "Live voting results with result bars",
 75:     title: "Live Results",
 76:     caption: "Vote totals and percentage bars update in real time.",
 77:   },
 78: ];
 79: 
 80: const slides = [
 81:   "/screenshots/Slide1.PNG",
 82:   "/screenshots/Slide2.PNG",
 83:   "/screenshots/Slide3.PNG",
 84:   "/screenshots/Slide4.PNG",
 85:   "/screenshots/Slide5.PNG",
 86:   "/screenshots/Slide6.PNG",
 87:   "/screenshots/Slide7.PNG",
 88: ];
 89: ---
 90: 
 91: <BaseLayout
 92:   title="Real-Time Voting System | Jared Street"
 93:   description="Node.js and Socket.IO voting system with live browser updates."
 94: >
 95:   <section class="page-hero project-hero fade-in">
 96:     <p class="eyebrow">JavaScript / Realtime</p>
 97:     <h1>Real-Time Voting System</h1>
 98:     <p>
 99:       A Node.js and Socket.IO project where users vote for a programming
100:       language and see poll results update instantly across connected browser
101:       clients.
102:     </p>
103: 
104:     <div class="tech-list">
105:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
106:     </div>
107: 
108:     <div class="button-row">
109:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
110:     </div>
111:   </section>
112: 
113:   <section class="section-card project-section fade-in">
114:     <p class="eyebrow">Overview</p>
115:     <h2>Project Purpose</h2>
116:     <p>
117:       The Real-Time Voting System demonstrates event-driven browser/server
118:       communication. Instead of requiring a page refresh, the server broadcasts
119:       updated vote totals to every connected client in real time.
120:     </p>
121:     <p>
122:       The project separates client and server logic. The client handles the
123:       voting interface and result bars, while the server maintains vote state,
124:       listens for Socket.IO events, and pushes updated totals to all users.
125:     </p>
126:   </section>
127: 
128:   <section class="section-card project-section fade-in">
129:     <p class="eyebrow">Features</p>
130:     <h2>What the Application Does</h2>
131: 
132:     <ul class="feature-list">
133:       {features.map((feature) => <li>{feature}</li>)}
134:     </ul>
135:   </section>
136: 
137:   <section class="section-card project-section fade-in">
138:     <p class="eyebrow">Code Sample</p>
139:     <h2>Socket.IO Server Events</h2>
140:     <p>
141:       This sample shows the server-side voting logic. When a client connects,
142:       votes, or resets the poll, the server updates state and broadcasts the new
143:       result totals to every connected browser.
144:     </p>
145: 
146:     <Code code={votingCode} lang="javascript" theme="github-dark" wrap />
147:   </section>
148: 
149:   <section class="section-card project-section fade-in">
150:     <p class="eyebrow">Screenshots</p>
151:     <h2>Application Screens</h2>
152: 
153:     <div class="screenshot-grid">
154:       {screenshots.map((screenshot) => (
155:         <figure class="screenshot-card">
156:           <img src={screenshot.src} alt={screenshot.alt} />
157:           <figcaption>
158:             <strong>{screenshot.title}</strong>
159:             <span>{screenshot.caption}</span>
160:           </figcaption>
161:         </figure>
162:       ))}
163:     </div>
164:   </section>
165: 
166:   <section class="section-card project-section fade-in">
167:     <p class="eyebrow">Presentation</p>
168:     <h2>Presentation Slides</h2>
169:     <p>
170:       These slides document the real-time voting project concept, technologies,
171:       team process, and application behavior.
172:     </p>
173: 
174:     <div class="screenshot-grid">
175:       {slides.map((slide, index) => (
176:         <figure class="screenshot-card">
177:           <img src={slide} alt={`Real-time voting presentation slide ${index + 1}`} />
178:           <figcaption>
179:             <strong>Slide {index + 1}</strong>
180:             <span>Presentation material for the real-time voting project.</span>
181:           </figcaption>
182:         </figure>
183:       ))}
184:     </div>
185:   </section>
186: </BaseLayout>
````

## File: src/pages/projects/wcf.astro
````astro
  1: ---
  2: import BaseLayout from "../../layouts/BaseLayout.astro";
  3: import { Code } from "astro:components";
  4: 
  5: const wcfCode = `[ServiceContract]
  6: public interface IService1
  7: {
  8:     [OperationContract]
  9:     void AddBook(Book book);
 10: 
 11:     [OperationContract]
 12:     void UpdateBook(Book book);
 13: 
 14:     [OperationContract]
 15:     void DeleteBook(int bookID);
 16: 
 17:     [OperationContract]
 18:     Book GetBook(int bookID);
 19: 
 20:     [OperationContract]
 21:     List<Book> GetAllBooks();
 22: 
 23:     [OperationContract]
 24:     List<Book> SearchByTitle(string title);
 25: 
 26:     [OperationContract]
 27:     List<Book> SearchByAuthor(string author);
 28: 
 29:     [OperationContract]
 30:     Book SearchByISBN(string isbn);
 31: 
 32:     [OperationContract]
 33:     bool CheckBookAvailability(int bookID);
 34: 
 35:     [OperationContract]
 36:     void CheckOutBook(int bookID);
 37: 
 38:     [OperationContract]
 39:     void ReturnBook(int bookID);
 40: }
 41: 
 42: [DataContract]
 43: public class Book
 44: {
 45:     [DataMember]
 46:     public int BookID { get; set; }
 47: 
 48:     [DataMember]
 49:     public string Title { get; set; }
 50: 
 51:     [DataMember]
 52:     public string Author { get; set; }
 53: 
 54:     [DataMember]
 55:     public string ISBN { get; set; }
 56: 
 57:     [DataMember]
 58:     public bool IsAvailable { get; set; }
 59: }`;
 60: 
 61: const techStack = [
 62:   "C#",
 63:   ".NET Framework 4.8",
 64:   "WCF",
 65:   "SOAP",
 66:   "Visual Studio 2022",
 67:   "Console Client",
 68: ];
 69: 
 70: const features = [
 71:   "Defines a WCF service contract with book management operations",
 72:   "Uses a Book data contract with book ID, title, author, ISBN, and availability fields",
 73:   "Adds new book records through the service",
 74:   "Updates existing book title, author, and ISBN data",
 75:   "Deletes books by book ID",
 76:   "Retrieves one book by book ID",
 77:   "Lists all books currently stored in the service",
 78:   "Searches books by title",
 79:   "Searches books by author",
 80:   "Searches for one book by ISBN",
 81:   "Checks whether a book is available",
 82:   "Checks out a book by changing its availability status",
 83:   "Returns a checked-out book by marking it available again",
 84:   "Uses WCF fault exceptions to report invalid input and missing records",
 85:   "Provides a menu-driven console client for testing service operations",
 86: ];
 87: 
 88: const screenshots = [
 89:   {
 90:     src: "/screenshots/library-wcf-service-browser.png",
 91:     alt: "Library WCF service running in browser",
 92:     title: "WCF Service Running in Browser",
 93:     caption: "The locally hosted WCF service running through the browser.",
 94:   },
 95:   {
 96:     src: "/screenshots/library-console-menu.png",
 97:     alt: "Library console application menu",
 98:     title: "Console Application Menu",
 99:     caption: "Menu-driven console client used to test service operations.",
100:   },
101:   {
102:     src: "/screenshots/library-console-output.png",
103:     alt: "Library console output showing book records",
104:     title: "Book Operation Output",
105:     caption: "Console output showing service responses for book operations.",
106:   },
107: ];
108: ---
109: 
110: <BaseLayout
111:   title="Library Record WCF Service | Jared Street"
112:   description="C# WCF service and console client for managing library book records."
113: >
114:   <section class="page-hero project-hero fade-in">
115:     <p class="eyebrow">C# / WCF</p>
116:     <h1>Library Record WCF Service</h1>
117:     <p>
118:       A C# web service project that defines a WCF service contract, exposes book
119:       management operations, and consumes those operations from a separate
120:       console client application.
121:     </p>
122: 
123:     <div class="tech-list">
124:       {techStack.map((tech) => <span class="tech-pill">{tech}</span>)}
125:     </div>
126: 
127:     <div class="button-row">
128:       <a class="button button-secondary" href="/projects/">Back to Projects</a>
129:     </div>
130:   </section>
131: 
132:   <section class="section-card project-section fade-in">
133:     <p class="eyebrow">Overview</p>
134:     <h2>Project Purpose</h2>
135:     <p>
136:       The Library Record WCF Service demonstrates structured service-based
137:       communication in C#. The solution includes a WCF service project that
138:       defines the service contract, data contract, and service implementation.
139:     </p>
140:     <p>
141:       A separate console client connects to the service through a generated
142:       service reference and provides a menu-driven interface for testing the
143:       library record operations.
144:     </p>
145:   </section>
146: 
147:   <section class="section-card project-section fade-in">
148:     <p class="eyebrow">Features</p>
149:     <h2>What the Service Does</h2>
150: 
151:     <ul class="feature-list">
152:       {features.map((feature) => <li>{feature}</li>)}
153:     </ul>
154:   </section>
155: 
156:   <section class="section-card project-section fade-in">
157:     <p class="eyebrow">Code Sample</p>
158:     <h2>Service Contract and Data Contract</h2>
159:     <p>
160:       This sample shows the operations exposed by the WCF service and the Book
161:       data contract passed between the service and the console client.
162:     </p>
163: 
164:     <Code code={wcfCode} lang="csharp" theme="github-dark" wrap />
165:   </section>
166: 
167:   <section class="section-card project-section fade-in">
168:     <p class="eyebrow">Screenshots</p>
169:     <h2>Application Screens</h2>
170: 
171:     <div class="screenshot-grid">
172:       {screenshots.map((screenshot) => (
173:         <figure class="screenshot-card">
174:           <img src={screenshot.src} alt={screenshot.alt} />
175:           <figcaption>
176:             <strong>{screenshot.title}</strong>
177:             <span>{screenshot.caption}</span>
178:           </figcaption>
179:         </figure>
180:       ))}
181:     </div>
182:   </section>
183: </BaseLayout>
````

## File: .gitignore
````
 1: # build output
 2: dist/
 3: # generated types
 4: .astro/
 5: 
 6: # dependencies
 7: node_modules/
 8: 
 9: # logs
10: npm-debug.log*
11: yarn-debug.log*
12: yarn-error.log*
13: pnpm-debug.log*
14: 
15: 
16: # environment variables
17: .env
18: .env.production
19: 
20: # macOS-specific files
21: .DS_Store
22: 
23: # jetbrains setting folder
24: .idea/
````

## File: astro.config.mjs
````javascript
1: // @ts-check
2: import { defineConfig } from 'astro/config';
3: 
4: // https://astro.build/config
5: export default defineConfig({});
````

## File: old-site/CIS_Syllabi.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="css/styles.css">
  7:     <title>CIS Course Syllabi</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="index.html">Home</a></li>
 14:             <li><a href="documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26:     <section class="syllabi-page">
 27:         
 28:     <section class="page-intro">
 29:         <p class="eyebrow">Academics</p>
 30:         <h2>CIS Course Syllabi</h2>
 31:         <p>
 32:             Course syllabi for CIS courses completed or currently in progress through
 33:             the Computer Programming program.
 34:         </p>
 35:     </section>
 36: 
 37:     <div class="syllabus-list">
 38:         <div class="syllabus-card">
 39:             <span class="course-code">CIS 130</span>
 40:             <span class="course-title">Introduction to Programming</span>
 41:             <a href="documents/syllabi/CIS130_syllabus.pdf">View Syllabus</a>
 42:         </div>
 43: 
 44:         <div class="syllabus-card">
 45:             <span class="course-code">CIS 195</span>
 46:             <span class="course-title">Internet Programming Essentials</span>
 47:             <a href="documents/syllabi/CIS195_syllabus.pdf">View Syllabus</a>
 48:         </div>
 49: 
 50:         <div class="syllabus-card">
 51:             <span class="course-code">CIS 194</span>
 52:             <span class="course-title">Introduction to Databases</span>
 53:             <a href="documents/syllabi/CIS194_syllabus.pdf">View Syllabus</a>
 54:         </div>
 55: 
 56:         <div class="syllabus-card">
 57:             <span class="course-code">CIS 196</span>
 58:             <span class="course-title">Internet Programming II</span>
 59:             <a href="documents/syllabi/CIS196_syllabus.pdf">View Syllabus</a>
 60:         </div>
 61: 
 62:         <div class="syllabus-card">
 63:             <span class="course-code">CIS 131</span>
 64:             <span class="course-title">C# Programming</span>
 65:             <a href="documents/syllabi/CIS131_syllabus.pdf">View Syllabus</a>
 66:         </div>
 67: 
 68:         <div class="syllabus-card">
 69:             <span class="course-code">CIS 137</span>
 70:             <span class="course-title">Data Analysis</span>
 71:             <a href="documents/syllabi/CIS137_syllabus.pdf">View Syllabus</a>
 72:         </div>
 73: 
 74:         <div class="syllabus-card">
 75:             <span class="course-code">CIS 241</span>
 76:             <span class="course-title">Dynamic Website Development</span>
 77:             <a href="documents/syllabi/CIS241_syllabus.pdf">View Syllabus</a>
 78:         </div>
 79: 
 80:         <div class="syllabus-card">
 81:             <span class="course-code">CIS 236</span>
 82:             <span class="course-title">Introduction to MS Web Development</span>
 83:             <a href="documents/syllabi/CIS236_syllabus.pdf">View Syllabus</a>
 84:         </div>
 85: 
 86:         <div class="syllabus-card">
 87:             <span class="course-code">CIS 225</span>
 88:             <span class="course-title">Secure Programming</span>
 89:             <a href="documents/syllabi/CIS225_syllabus.pdf">View Syllabus</a>
 90:         </div>
 91: 
 92:         <div class="syllabus-card">
 93:             <span class="course-code">CIS 279</span>
 94:             <span class="course-title">Databases II</span>
 95:             <a href="documents/syllabi/CIS279_syllabus.pdf">View Syllabus</a>
 96:         </div>
 97: 
 98:         <div class="syllabus-card">
 99:             <span class="course-code">CIS 266</span>
100:             <span class="course-title">Web Services</span>
101:             <a href="documents/syllabi/CIS266_syllabus.pdf">View Syllabus</a>
102:         </div>
103: 
104:         <div class="syllabus-card">
105:             <span class="course-code">CIS 293</span>
106:             <span class="course-title">Advanced Technologies</span>
107:             <a href="documents/syllabi/CIS293_syllabus.pdf">View Syllabus</a>
108:         </div>
109: 
110:         <div class="syllabus-card">
111:             <span class="course-code">CIS 296</span>
112:             <span class="course-title">MS Web Development II</span>
113:             <a href="documents/syllabi/CIS296_syllabus.pdf">View Syllabus</a>
114:         </div>
115: 
116:         <div class="syllabus-card">
117:             <span class="course-code">CIS 207</span>
118:             <span class="course-title">eBusiness</span>
119:             <a href="documents/syllabi/CIS207_syllabus.pdf">View Syllabus</a>
120:         </div>
121: 
122:         <div class="syllabus-card">
123:             <span class="course-code">CIS 248</span>
124:             <span class="course-title">Advanced Application Development</span>
125:             <a href="documents/syllabi/CIS248_syllabus.pdf">View Syllabus</a>
126:         </div>
127:     </div>
128:     </section>
129:     <footer>
130:         <p>&copy; 2026 Jared Street | CIS 266 Electronic Portfolio</p>
131:     </footer>
132: </body>
133: </html>
````

## File: old-site/cis241.html
````html
 1: <!DOCTYPE html>
 2: <html lang="en">
 3: <head>
 4:     <meta charset="UTF-8">
 5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
 6:     <title>Jared Street - CIS 241 Projects</title>
 7:     <link rel="stylesheet" href="css/styles.css">
 8: </head>
 9: 
10: <body>
11:     <header>
12:         <nav>
13:             <a href="index.html" class="brand">Jared Street</a>
14:             <ul>
15:                 <li><a href="index.html">Home</a></li>
16:                 <li><a href="documents/JaredStreetResume.pdf">Resume</a></li>
17:                 <li><a href="CIS_Syllabi.html">CIS Syllabi</a></li>
18:                 <li><a href="cis241.html">CIS 241 Projects</a></li>
19:                 <li><a href="cis266.html">CIS 266 Web Services</a></li>
20:                 <li><a href="cis296.html">CIS 296 C# Projects</a></li>
21:                 <li>
22:                     <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
23:                         STI CIS Curriculum
24:                     </a>
25:                 </li>
26:             </ul>
27:         </nav>
28:     </header>
29: 
30:     <main>
31:         <section>
32:             <h2>CIS 241 - Dynamic Website Development Projects</h2>
33:             <p>
34:                 This page includes dynamic website projects completed for CIS 241.
35:                 These projects demonstrate PHP, MySQL, server-side programming,
36:                 database interaction, and dynamic page behavior.
37:             </p>
38:         </section>
39: 
40:         <section>
41:             <h2>Project Samples</h2>
42: 
43:             <article>
44:                 <h3>Simple Forum Application</h3>
45: 
46:                 <p>
47:                     A dynamic PHP/MySQL forum application where users can register,
48:                     log in, browse categories, create posts, edit posts, and delete posts.
49:                     The project demonstrates database-backed web development using PHP,
50:                     MySQL/MariaDB, PDO, sessions, and Bootstrap.
51:                 </p>
52: 
53:                 <p>
54:                     <strong>Technologies:</strong>
55:                     PHP, MySQL, PDO, HTML, CSS, Bootstrap
56:                 </p>
57: 
58:                 <p>
59:                     <a href="projects/simple-forum.html">View Project Documentation</a>
60:                 </p>
61: 
62:                 <p>
63:                     <a href="https://cis241simpleforum.ct.ws/index.php" target="_blank" rel="noopener noreferrer">
64:                         View Live PHP/MySQL Demo
65:                     </a>
66:                 </p>
67:             </article>
68:         </section>
69:     </main>
70: 
71:     <footer>
72:         <p>&copy; 2026 Jared Street | CIS 266 Electronic Portfolio</p>
73:     </footer>
74: </body>
75: </html>
````

## File: old-site/cis266.html
````html
 1: <!DOCTYPE html>
 2: <html lang="en">
 3: <head>
 4:     <meta charset="UTF-8">
 5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
 6:     <title>Jared Street - CIS 266 Web Services Projects</title>
 7:     <link rel="stylesheet" href="css/styles.css">
 8: </head>
 9: 
10: <body>
11:     <header>
12:         <nav>
13:             <a href="index.html" class="brand">Jared Street</a>
14:             <ul>
15:                 <li><a href="index.html">Home</a></li>
16:                 <li><a href="documents/JaredStreetResume.pdf">Resume</a></li>
17:                 <li><a href="CIS_Syllabi.html">CIS Syllabi</a></li>
18:                 <li><a href="cis241.html">CIS 241 Projects</a></li>
19:                 <li><a href="cis266.html">CIS 266 Web Services</a></li>
20:                 <li><a href="cis296.html">CIS 296 C# Projects</a></li>
21:                 <li>
22:                     <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
23:                         STI CIS Curriculum
24:                     </a>
25:                 </li>
26:             </ul>
27:         </nav>
28:     </header>
29: 
30:     <main>
31:         <section>
32:             <h2>CIS 266 - Web Services Projects</h2>
33:             <p>
34:                 This page includes project documentation for CIS 266 Web Services,
35:                 including RESTful PHP/MySQL services, AJAX/JSON clients, WCF services,
36:                 and team project demonstrations.
37:             </p>
38:         </section>
39: 
40:         <section>
41:             <h2>Project Samples</h2>
42: 
43:             <article>
44:                 <h3>Unit2_Ex3 RESTful AJAX-JSON-PHP-MySQL Web Service</h3>
45:                 <p>
46:                     A REST-style PHP/MySQL web service using JSON data and AJAX client-side requests.
47:                 </p>
48:                 <p><strong>Technologies:</strong> PHP, MySQL, JSON, AJAX, JavaScript, HTML, CSS</p>
49:                 <p><a href="projects/RESTful-AJAX-JSON-PHP-MySQL.html">View Project Documentation</a></p>
50:             </article>
51: 
52:             <article>
53:                 <h3>Scrum 3 Team Project - CRUD RESTful Web Service</h3>
54:                 <p>
55:                     A team-built CRUD web service using PHP, MySQL, JSON, and client-side JavaScript.
56:                 </p>
57:                 <p><strong>Technologies:</strong> PHP, MySQL, JSON, JavaScript, AJAX, HTML, CSS</p>
58:                 <p><a href="projects/CRUD-RESTful-service.html">View Project Documentation</a></p>
59:             </article>
60: 
61:             <article>
62:                 <h3>Unit3 WCF Project</h3>
63:                 <p>
64:                     A static project documentation page for a WCF service and client application.
65:                 </p>
66:                 <p><strong>Technologies:</strong> C#, WCF, SOAP, Visual Studio, .NET Framework</p>
67:                 <p><a href="projects/wcf.html">View Project Documentation</a></p>
68:             </article>
69: 
70:             <article>
71:                 <h3>Scrum 4 Team Project - Presentation and Demo Videos</h3>
72:                 <p>
73:                     Team project materials including presentation slides and demo videos.
74:                 </p>
75:                 <p><strong>Technologies:</strong> Node.js, Socket.IO, JavaScript, HTML, CSS</p>
76:                 <p><a href="projects/voting-system.html">View Project Materials</a></p>
77:             </article>
78:         </section>
79:     </main>
80: 
81:     <footer>
82:         <p>&copy; 2026 Jared Street | CIS 266 Electronic Portfolio</p>
83:     </footer>
84: </body>
85: </html>
````

## File: old-site/cis296.html
````html
 1: <!DOCTYPE html>
 2: <html lang="en">
 3: <head>
 4:     <meta charset="UTF-8">
 5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
 6:     <title>Jared Street - CIS 296 C# Projects</title>
 7:     <link rel="stylesheet" href="css/styles.css">
 8: </head>
 9: 
10: <body>
11:     <header>
12:         <nav>
13:             <a href="index.html" class="brand">Jared Street</a>
14:             <ul>
15:                 <li><a href="index.html">Home</a></li>
16:                 <li><a href="documents/JaredStreetResume.pdf">Resume</a></li>
17:                 <li><a href="CIS_Syllabi.html">CIS Syllabi</a></li>
18:                 <li><a href="cis241.html">CIS 241 Projects</a></li>
19:                 <li><a href="cis266.html">CIS 266 Web Services</a></li>
20:                 <li><a href="cis296.html">CIS 296 C# Projects</a></li>
21:                 <li>
22:                     <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
23:                         STI CIS Curriculum
24:                     </a>
25:                 </li>
26:             </ul>
27:         </nav>
28:     </header>
29: 
30:     <main>
31:         <section>
32:             <h2>CIS 296 - Advanced C# Projects</h2>
33:             <p>
34:                 This page includes documentation for advanced C# project work completed
35:                 in CIS 296. The selected project includes a description, screenshots,
36:                 and sample code.
37:             </p>
38:         </section>
39: 
40:         <section>
41:             <h2>Project Sample</h2>
42: 
43:             <article>
44:                 <h3>SportsPro Technical Support</h3>
45:                 <p>
46:                     This is an ASP.NET Core MVC application built for CIS 296. The project demonstrates a database-backed support management system where users can maintain product, customer, technician, and incident records through standard MVC list, add, edit, and delete workflows.
47:                 </p>
48: 
49:                 <p>
50:                     <strong>Technologies:</strong>
51:                     C#, ASP.NET Core MVC, Entity Framework Core, SQL Server
52:                 </p>
53: 
54:                 <p>
55:                     <a href="projects/sportspro.html">View Project Documentation</a>
56:                 </p>
57:             </article>
58:         </section>
59:     </main>
60: 
61:     <footer>
62:         <p>&copy; 2026 Jared Street | CIS 266 Electronic Portfolio</p>
63:     </footer>
64: </body>
65: </html>
````

## File: old-site/css/styles.css
````css
  1: :root {
  2:     --bg: #0f172a;
  3:     --panel: #111827;
  4:     --border: #334155;
  5:     --text: #e5e7eb;
  6:     --muted: #94a3b8;
  7:     --accent: #facc15;
  8:     --link: #60a5fa;
  9: }
 10: 
 11: body {
 12:     font-family: Arial, Helvetica, sans-serif;
 13: }
 14: 
 15: h1,
 16: h2,
 17: h3 {
 18:     font-family: "Trebuchet MS", Arial, Helvetica, sans-serif;
 19:     letter-spacing: 0.02em;
 20: }
 21: 
 22: nav,
 23: button,
 24: .syllabus-card a {
 25:     font-family: Arial, Helvetica, sans-serif;
 26: }
 27: 
 28: pre,
 29: code {
 30:     font-family: Consolas, Monaco, "Courier New", monospace;
 31: }
 32: 
 33: html, body {
 34:     min-height: 100%;
 35: }
 36: 
 37: body {
 38:     margin: 0;
 39:     min-height: 100vh;
 40:     display: flex;
 41:     flex-direction: column;
 42:     font-family: Arial, Helvetica, sans-serif;
 43:     background-color: #0f172a;
 44:     color: #e5e7eb;
 45:     line-height: 1.6;
 46: }
 47: 
 48: main {
 49:     flex: 1;
 50:     max-width: 1200px;
 51:     width: 100%;
 52:     margin: 2rem auto;
 53:     padding: 0 2rem;
 54: }
 55: 
 56: header {
 57:     background-color: #111827;
 58:     color: white;
 59:     padding: 2rem 1rem;
 60:     text-align: center;
 61: }
 62: 
 63: nav {
 64:     background-color: #111827;
 65:     border-bottom: 3px solid #2563eb;
 66: }
 67: 
 68: nav .brand {
 69:     display: block;
 70:     color: white;
 71:     font-weight: bold;
 72:     text-decoration: none;
 73:     padding: 1rem;
 74:     text-align: center;
 75:     font-size: 1.2rem;
 76: }
 77: 
 78: nav ul {
 79:     list-style: none;
 80:     margin: 0;
 81:     padding: 0 1rem 1rem;
 82:     display: flex;
 83:     justify-content: center;
 84:     flex-wrap: wrap;
 85:     gap: 1rem;
 86: }
 87: 
 88: nav a {
 89:     color: #e5e7eb;
 90:     text-decoration: none;
 91: }
 92: 
 93: nav a:hover {
 94:     color: white;
 95:     text-decoration: underline;
 96: }
 97: 
 98: section,
 99: article {
100:     background-color: #111827;
101:     border: 1px solid #334155;
102:     border-radius: 10px;
103:     padding: 1.5rem;
104:     margin-bottom: 1.5rem;
105: }
106: 
107: article {
108:     box-shadow: 0 2px 8px rgba(0, 0, 0, 0.06);
109: }
110: 
111: img {
112:     max-width: 100%;
113:     height: auto;
114:     border: 1px solid #334155;
115:     border-radius: 10px;
116:     display: block;
117: }
118: 
119: figure {
120:     margin: 1.5rem 0 2rem;
121: }
122: 
123: figcaption {
124:     font-size: 0.95rem;
125:     color: #94a3b8;
126:     margin-top: 0.5rem;
127: }
128: 
129: pre {
130:     background-color: #02050e;
131:     color: #f9fafb;
132:     padding: 1rem;
133:     border-radius: 8px;
134:     overflow-x: auto;
135: }
136: 
137: code {
138:     font-family: Consolas, Monaco, monospace;
139: }
140: 
141: footer {
142:     text-align: center;
143:     background-color: #111827;
144:     color: white;
145:     padding: 1rem;
146:     margin-top: 2rem;
147: }
148: 
149: a {
150:     color: #60a5fa;
151: }
152: 
153: a:hover {
154:     color: #93c5fd;
155: }
156: 
157: main a {
158:     font-weight: bold;
159: }
160: 
161: .syllabi-page {
162:     background-color: transparent;
163:     border: none;
164:     padding: 0;
165: }
166: 
167: .syllabus-list {
168:     display: grid;
169:     gap: 1rem;
170:     max-width: 1200px;
171:     margin: 0 auto;
172: }
173: 
174: .syllabus-card {
175:     display: grid;
176:     grid-template-columns: 100px 1fr auto;
177:     align-items: center;
178:     gap: 1rem;
179: 
180:     background-color: #111827;
181:     border: 1px solid #334155;
182:     border-radius: 10px;
183:     padding: 1rem 1.25rem;
184: }
185: 
186: h1, h3 {
187:     color: #facc15;
188: }
189: 
190: p,
191: li {
192:     color: #e5e7eb;
193: }
194: 
195: .course-code {
196:     color: #facc15;
197:     font-weight: bold;
198:     letter-spacing: 0.05em;
199: }
200: 
201: .course-title {
202:     color: #e5e7eb;
203:     font-weight: 600;
204: }
205: 
206: .syllabus-card a {
207:     border: 1px solid #facc15;
208:     color: #facc15;
209:     padding: 0.4rem 0.75rem;
210:     border-radius: 6px;
211:     text-decoration: none;
212:     font-size: 0.9rem;
213: }
214: 
215: .syllabus-card a:hover {
216:     background-color: #facc15;
217:     color: #111827;
218: }
219: 
220: @media (max-width: 700px) {
221:     .syllabus-card {
222:         grid-template-columns: 1fr;
223:         align-items: start;
224:     }
225: 
226:     .syllabus-card a {
227:         width: fit-content;
228:     }
229: }
230: 
231: .page-intro {
232:     background-color: transparent;
233:     border: none;
234:     max-width: 1200px;
235:     margin: 0 auto;
236:     padding: 2rem 0;
237: }
238: 
239: .eyebrow {
240:     color: #facc15;
241:     text-transform: uppercase;
242:     letter-spacing: 0.2em;
243:     font-size: 0.85rem;
244:     font-weight: bold;
245: }
246: 
247: .project-documentation {
248:     max-width: 1200px;
249:     margin: 2rem auto;
250:     padding: 1rem 1.25rem;
251: }
````

## File: old-site/index.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <title>Jared Street - Electronic Portfolio</title>
  7:     <link rel="stylesheet" href="css/styles.css">
  8: </head>
  9: 
 10: <body>
 11:     <header>
 12:         <h1>Jared Street</h1>
 13:         <p>CIS Student - Southeast Technical Institute </p>
 14: 
 15:         <nav>
 16:             <ul>
 17:                 <li><a href="index.html">Home</a></li>
 18:                 <li><a href="documents/JaredStreetResume.pdf">Resume</a></li>
 19:                 <li><a href="CIS_Syllabi.html">CIS Syllabi</a></li>
 20:                 <li><a href="cis241.html">CIS 241 Projects</a></li>
 21:                 <li><a href="cis266.html">CIS 266 Web Services</a></li>
 22:                 <li><a href="cis296.html">CIS 296 C# Projects</a></li>
 23:                 <li>
 24:                     <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 25:                         STI CIS Curriculum
 26:                     </a>
 27:                 </li>
 28:             </ul>
 29:         </nav>
 30:     </header>
 31: 
 32:     <main>
 33:         <section id="welcome">
 34:             <h2>Welcome</h2>
 35:             <p>
 36:                 My portfolio presents selected coursework, project documentation,
 37:                 and technical skills I completed through the Computer Programming program at
 38:                 Southeast Technical Institute. You can also find my resume, and links to syllabi for completed courses.
 39:             </p>
 40:         </section>
 41: 
 42:         <section id="portfolio-sections">
 43:             <h2>Portfolio</h2>
 44: 
 45:             <article>
 46:                 <p>
 47:                     <a href="documents/JaredStreetResume.pdf"><h3>Resume</h3></a>
 48:                 </p>
 49:             </article>
 50: 
 51:             <article>
 52:                 <p>
 53:                     <a href="CIS_Syllabi.html"><h3>CIS Course Syllabi</h3></a>
 54:                 </p>
 55:             </article>
 56: 
 57:             <article>
 58:                 <h3>Dynamic Projects</h3>
 59:                 <p>
 60:                     This section includes documentation for dynamic web projects, including
 61:                     a working PHP/MySQL database demonstration.
 62:                 </p>
 63:                 <p>
 64:                     <a href="cis241.html">View Dynamic Projects</a>
 65:                 </p>
 66:             </article>
 67: 
 68:             <article>
 69:                 <h3>Web Services Projects</h3>
 70:                 <p>
 71:                     This section includes RESTful web service, AJAX, JSON, PHP/MySQL, WCF,
 72:                     and team project documentation from CIS 266.
 73:                 </p>
 74:                 <p>
 75:                     <a href="cis266.html">View Web Services Projects</a>
 76:                 </p>
 77:             </article>
 78: 
 79:             <article>
 80:                 <h3>Advanced C# Projects</h3>
 81:                 <p>
 82:                     This section includes documentation for advanced C# project work, including
 83:                     project descriptions, screenshots, and sample code.
 84:                 </p>
 85:                 <p>
 86:                     <a href="cis296.html">View C# Projects</a>
 87:                 </p>
 88:             </article>
 89: 
 90:             <article>
 91:                 <p>
 92:                     <a href="projects.html">View Other Projects</a>
 93:                 </p>
 94:             </article>
 95:         </section>
 96: 
 97:         <section id="program-link">
 98:             <h2>Program Curriculum</h2>
 99:             <p>
100:                 More information about the Southeast Technical Institute Computer Programming
101:                 curriculum is available through the official program page.
102:             </p>
103:             <p>
104:                 <a href="https://catalog.southeasttech.edu/preview_program.php?catoid=28&poid=3469&returnto=20031">
105:                     View STI CIS Computer Programming Curriculum
106:                 </a>
107:             </p>
108:         </section>
109:     </main>
110: 
111:     <footer>
112:         <p>&copy; 2026 Jared Street | CIS 266 Electronic Portfolio</p>
113:     </footer>
114: </body>
115: </html>
````

## File: old-site/projects.html
````html
 1: <!DOCTYPE html>
 2: <html lang="en">
 3: <head>
 4:     <meta charset="UTF-8">
 5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
 6:     <title>Jared Street - Featured Advanced Project</title>
 7:     <link rel="stylesheet" href="css/styles.css">
 8: </head>
 9: 
10: <body>
11:     <header>
12:         <h1>Jared Street</h1>
13:         <p>CIS Student - Southeast Technical Institute</p>
14: 
15:         <nav>
16:             <a href="index.html" class="brand">Jared Street</a>
17:             <ul>
18:                 <li><a href="index.html">Home</a></li>
19:                 <li><a href="documents/JaredStreetResume.pdf">Resume</a></li>
20:                 <li><a href="CIS_Syllabi.html">CIS Syllabi</a></li>
21:                 <li><a href="cis241.html">CIS 241 Projects</a></li>
22:                 <li><a href="cis266.html">CIS 266 Web Services</a></li>
23:                 <li><a href="cis296.html">CIS 296 C# Projects</a></li>
24:                 <li>
25:                     <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
26:                         STI CIS Curriculum
27:                     </a>
28:                 </li>
29:             </ul>
30:         </nav>
31:     </header>
32: 
33:     <main>
34:         <section>
35:             <h2>Other Projects</h2>
36:             <p>
37:                 This page includes documentation for other projects I completed during my coursework.
38:             </p>
39:         </section>
40: 
41:         <section>
42:             <h2>Project Samples</h2>
43: 
44:             <article>
45:                 <h3>Display Switching CLI Tool</h3>
46:                 <p>
47:                     A Go console application that allows users to switch between multiple
48:                     display configurations on their computer.
49:                 </p>
50: 
51:                 <p>
52:                     <strong>Technologies:</strong>
53:                     Go, Cobra CLI framework, MultiMonitor API, JSON configuration
54:                 </p>
55: 
56:                 <p>
57:                     <a href="projects/switcher.html">View Project Documentation</a>
58:                 </p>
59:             </article>
60: 
61:             <article>
62:                 <h3>Godot Roguelike Prototype</h3>
63:                 <p>
64:                     A simple roguelike game prototype built with the Godot game engine.
65:                 </p>
66: 
67:                 <p>
68:                     <strong>Technologies:</strong>
69:                     Godot, C#
70:                 </p>
71: 
72:                 <p>
73:                     <a href="projects/godot-roguelike.html">View Project Documentation</a>
74:                 </p>
75:             </article>
76:         </section>
77:     </main>
78: 
79:     <footer>
80:         <p>&copy; 2026 Jared Street | CIS 266 Electronic Portfolio</p>
81:     </footer>
82: </body>
83: </html>
````

## File: old-site/projects/CRUD-RESTful-service.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>Dark Souls CRUD Web Service - CIS 266</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>Dark Souls CRUD Web Service</h1>
 29: 
 30:         <p>
 31:             The Dark Souls CRUD Web Service is a PHP/MySQL web service project built for
 32:             CIS 266. The project demonstrates a themed full CRUD application where the
 33:             browser client communicates with a PHP API to create, read, update, and delete
 34:             records from a MySQL database.
 35:         </p>
 36: 
 37:         <p>
 38:             The application separates the client and provider portions of the project. The
 39:             provider side contains the PHP API, database class, object classes, SQL export,
 40:             and tester page. The client side contains the HTML interface, JavaScript AJAX
 41:             logic, CSS styling, sound effects, and particle animation used to create a
 42:             Dark Souls-inspired user experience.
 43:         </p>
 44: 
 45:         <h2>Technologies Used</h2>
 46: 
 47:         <ul>
 48:             <li>PHP</li>
 49:             <li>MySQL</li>
 50:             <li>phpMyAdmin SQL export</li>
 51:             <li>Object-oriented PHP classes</li>
 52:             <li>HTML</li>
 53:             <li>CSS</li>
 54:             <li>JavaScript</li>
 55:             <li>jQuery AJAX</li>
 56:             <li>JSON</li>
 57:             <li>Draw.io UML diagram</li>
 58:             <li>Localhost / WAMP-style development environment</li>
 59:         </ul>
 60: 
 61:         <h2>Features</h2>
 62: 
 63:         <ul>
 64:             <li>Provides a PHP API endpoint for CRUD operations</li>
 65:             <li>Supports reading, inserting, updating, and deleting records</li>
 66:             <li>Uses a MySQL database named <code>darksouls</code></li>
 67:             <li>Stores data in <code>characters</code>, <code>factions</code>, and <code>weapons</code> tables</li>
 68:             <li>Uses PHP classes for Character, Faction, Weapon, and database access logic</li>
 69:             <li>Returns API responses as JSON</li>
 70:             <li>Uses jQuery AJAX requests to communicate with the API</li>
 71:             <li>Displays live table data for characters, factions, and weapons</li>
 72:             <li>Includes form controls for CRUD operations on each table</li>
 73:             <li>Uses animation effects for inserted, updated, and deleted rows</li>
 74:             <li>Includes sound effects for insert, update, and delete actions</li>
 75:             <li>Includes ember particle animation and Dark Souls-inspired styling</li>
 76:             <li>Includes an SQL export for recreating the database structure and sample data</li>
 77:             <li>Includes a UML diagram showing the project classes and relationships</li>
 78:         </ul>
 79: 
 80:         <h2>Code Sample</h2>
 81: 
 82:         <p>
 83:             This sample shows the main PHP API controller for the project. The script receives
 84:             an <code>action</code> and <code>table</code> value from the request, calls the matching
 85:             database method, and returns a JSON response to the client.
 86:         </p>
 87: 
 88:         <pre><code class="language-php">&lt;?php
 89: 
 90: include_once('classes/Character.php');
 91: include_once('classes/Faction.php');
 92: include_once('classes/Weapon.php');
 93: 
 94: header('Content-Type: application/json');
 95: 
 96: include_once('classes/DB_200.php');
 97: $db = new DB_200();
 98: 
 99: $action = $_REQUEST['action'];
100: $table = $_REQUEST['table'];
101: 
102: // READ
103: if ($action == "read") {
104:     $id = !empty($_REQUEST['id']) ? $_REQUEST['id'] : null;
105:     $result = $db-&gt;read($table, $id);
106:     $data = [];
107: 
108:     while ($row = $result-&gt;fetch_assoc()) {
109:         if ($table === "characters") {
110:             $obj = new Character(
111:                 $row["id"],
112:                 $row["name"],
113:                 $row["class"],
114:                 $row["level"],
115:                 $row["faction_id"],
116:                 $row["weapon_id"]
117:             );
118:         } elseif ($table === "factions") {
119:             $obj = new Faction(
120:                 $row["id"],
121:                 $row["name"],
122:                 $row["alignment"],
123:                 $row["leader"],
124:                 $row["territory"]
125:             );
126:         } elseif ($table === "weapons") {
127:             $obj = new Weapon(
128:                 $row["id"],
129:                 $row["name"],
130:                 $row["damage"],
131:                 $row["scaling"],
132:                 $row["weight"]
133:             );
134:         }
135: 
136:         $data[] = $obj-&gt;toArray();
137:     }
138: 
139:     echo json_encode($data);
140: }
141: 
142: // INSERT
143: if ($action == "insert") {
144:     $data = $_POST;
145:     unset($data['action'], $data['table']);
146:     $db-&gt;insert($table, $data);
147:     echo json_encode(["status" =&gt; "inserted"]);
148: }
149: 
150: // UPDATE
151: if ($action == "update") {
152:     $id = $_POST['id'];
153:     $data = $_POST;
154:     unset($data['action'], $data['table'], $data['id']);
155:     $data = array_filter($data, function($value) {
156:         return $value !== "";
157:     });
158:     $db-&gt;update($table, $id, $data);
159:     echo json_encode(["status" =&gt; "updated"]);
160: }
161: 
162: // DELETE
163: if ($action == "delete") {
164:     $id = $_REQUEST['id'];
165:     $db-&gt;delete($table, $id);
166:     echo json_encode(["status" =&gt; "deleted"]);
167: }
168: 
169: ?&gt;</code></pre>
170: 
171:         <p>
172:             This file represents the main API pattern used by the application: receive a request
173:             from the client, determine the requested CRUD action, call the database layer, and
174:             return a JSON response that the JavaScript client can display.
175:         </p>
176: 
177:         <h2>App Screen Captures</h2>
178: 
179:         <h3>Dark Souls CRUD Home Page</h3>
180:         <figure>
181:             <img src="screenshots/darksouls-home.png" alt="Dark Souls CRUD web service home page">
182:             <figcaption>Client interface for the Dark Souls-themed CRUD web service.</figcaption>
183:         </figure>
184: 
185:         <h3>Live table viewer</h3>
186:         <figure>
187:             <img src="screenshots/darksouls-live-table.png" alt="Live database display">
188:             <figcaption>This is the live table of the database. CRUD operations are reflected in real-time.</figcaption>
189:         </figure>
190: 
191:         <h3>Database API display</h3>
192:         <figure>
193:             <img src="screenshots/darksouls-database-display-API.png" alt="Entire database displayed through the API">
194:             <figcaption>This is the entire database displayed through the API.</figcaption>
195:         </figure>
196: 
197:         <p>
198:             <a href="../cis266.html">Back to CIS 266 Projects</a>
199:         </p>
200:     </section>
201: 
202: 
203: </body>
204: </html>
````

## File: old-site/projects/godot-roguelike.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>Godot Grid Roguelike Prototype - Project Documentation</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>Godot Grid Roguelike Prototype</h1>
 29: 
 30:         <p>
 31:             The Godot Grid Roguelike Prototype is a turn-based dungeon crawler built in
 32:             Godot 4.4.1 with C#. The project focuses on grid-based movement, player and
 33:             enemy combat, floor progression, rewards, persistent run data, and basic game
 34:             flow from the start menu through victory or game over.
 35:         </p>
 36: 
 37:         <p>
 38:             The prototype uses a scene-based structure with separate scenes for the start
 39:             menu, combat floors, reward selection, game over, and victory. Combat takes place
 40:             on tile-based maps where the player moves one grid cell at a time, attacks enemies
 41:             by bumping into them, and then waits while enemies resolve their turns. Between
 42:             non-boss floors, the player chooses rewards that modify stats, grant boons, or
 43:             equip gear for the rest of the run.
 44:         </p>
 45: 
 46:         <h2>Technologies Used</h2>
 47: 
 48:         <ul>
 49:             <li>Godot 4.4.1</li>
 50:             <li>C#</li>
 51:             <li>.NET / Godot C# project structure</li>
 52:             <li>Godot scenes and nodes</li>
 53:             <li>TileMapLayer-based level design</li>
 54:             <li>Node2D gameplay objects</li>
 55:             <li>Godot autoload-style persistent run state</li>
 56:             <li>RichTextLabel UI logging</li>
 57:             <li>AudioStreamPlayer sound effects</li>
 58:             <li>Custom pixel-art assets and imported textures</li>
 59:             <li>Custom UI themes and style resources</li>
 60:         </ul>
 61: 
 62:         <h2>Features</h2>
 63: 
 64:         <ul>
 65:             <li>Turn-based grid movement using keyboard input</li>
 66:             <li>Tile-based collision and walkability checks</li>
 67:             <li>Player bump-attacks when moving into an occupied enemy tile</li>
 68:             <li>Sequential enemy turn resolution after the player acts</li>
 69:             <li>Enemy movement and adjacency-based attacks</li>
 70:             <li>Multiple combat floors with a final boss floor</li>
 71:             <li>Reward selection between non-boss floors</li>
 72:             <li>Persistent run state across scene changes</li>
 73:             <li>Player stats for health, max health, damage, enemies defeated, and total damage dealt</li>
 74:             <li>Active abilities including Whirlwind, Attack Buff, and Heal</li>
 75:             <li>Passive reward effects such as healing on kill, regeneration, and scaling damage bonuses</li>
 76:             <li>Gear rewards such as Iron Charm and Rage Mask</li>
 77:             <li>Combat log using styled RichTextLabel text</li>
 78:             <li>Sound effects for player attacks, enemy attacks, deaths, hits, and floor clear events</li>
 79:             <li>Start menu, reward screen, game over screen, and victory screen</li>
 80:             <li>Custom art assets for player, enemies, boss, terrain, walls, stairs, and environmental tiles</li>
 81:         </ul>
 82: 
 83:         <h2>Code Sample</h2>
 84: 
 85:         <p>
 86:             This sample shows the derived stat and passive-effect logic from the project.
 87:             The <code>RunEffects</code> class calculates effective health and damage based on
 88:             the current run state, then applies reward effects such as healing on kill or
 89:             gaining permanent damage after defeating enough enemies.
 90:         </p>
 91: 
 92:         <pre><code class="language-csharp">public static class RunEffects
 93: {
 94:     public static int GetEffectiveMaxHealth(Player player, RunState runState)
 95:     {
 96:         int maxHealth = runState.BaseMaxHealth;
 97: 
 98:         if (runState.CurrentGear == RunState.GearType.IronCharm)
 99:             maxHealth += 15;
100: 
101:         return maxHealth;
102:     }
103: 
104:     public static int GetEffectiveDamage(Player player, RunState runState)
105:     {
106:         int damage = runState.BaseDamage;
107: 
108:         if (runState.CurrentGear == RunState.GearType.RageMask &amp;&amp;
109:             player.Health * 2 &lt; GetEffectiveMaxHealth(player, runState))
110:         {
111:             damage += 2;
112:         }
113: 
114:         if (player.NextAttackBuffed)
115:         {
116:             damage *= 2;
117:         }
118: 
119:         return damage;
120:     }
121: 
122:     public static void OnEnemyKilled(Player player, RunState runState, Start map)
123:     {
124:         if (runState.OwnedBoons.Contains(RunState.BoonType.HealOnKill))
125:         {
126:             player.Health = Math.Min(
127:                 player.Health + 1,
128:                 GetEffectiveMaxHealth(player, runState)
129:             );
130: 
131:             map.AddLogMessageRaw(
132:                 $"[color=green]Life Tap[/color] restores [color=green]1 HP[/color]."
133:             );
134:         }
135: 
136:         if (runState.OwnedBoons.Contains(RunState.BoonType.CrushingWeight))
137:         {
138:             int newTier = runState.EnemiesDefeated / 5;
139: 
140:             if (newTier &gt; runState.CrushingWeightTiersAwarded)
141:             {
142:                 int tiersGained = newTier - runState.CrushingWeightTiersAwarded;
143:                 runState.BaseDamage += tiersGained;
144:                 runState.CrushingWeightTiersAwarded = newTier;
145: 
146:                 map.AddLogMessageRaw(
147:                     $"[color=orange]Crushing Weight[/color] grants " +
148:                     $"[color=yellow]+{tiersGained} damage[/color]."
149:                 );
150:             }
151:         }
152: 
153:         SyncPlayerStats(player, runState);
154:     }
155: }</code></pre>
156: 
157:         <p>
158:             This code represents one of the main roguelike systems in the project: rewards
159:             and gear do not just change the UI; they affect combat calculations and carry
160:             forward through the persistent run state.
161:         </p>
162: 
163:         <h2>App Screen Captures</h2>
164: 
165:         <h3>Start Menu</h3>
166:         <figure>
167:             <img src="screenshots/roguelike-start-menu.png" alt="Godot roguelike start menu">
168:             <figcaption>Start menu used to begin a new run.</figcaption>
169:         </figure>
170: 
171:         <h3>Combat Floor</h3>
172:         <figure>
173:             <img src="screenshots/roguelike-combat-floor.png" alt="Godot roguelike combat floor with player and enemies">
174:             <figcaption>Grid-based combat floor with player movement, enemies, UI, and combat log.</figcaption>
175:         </figure>
176: 
177:         <h3>Reward Selection</h3>
178:         <figure>
179:             <img src="screenshots/roguelike-reward-selection.png" alt="Godot roguelike reward selection screen">
180:             <figcaption>Reward cards presented between floors to improve the current run.</figcaption>
181:         </figure>
182: 
183:         <h3>Final Floor</h3>
184:         <figure>
185:             <img src="screenshots/roguelike-final-floor.png" alt="Godot roguelike final floor">
186:             <figcaption>Final floor before the end screen.</figcaption>
187:         </figure>
188: 
189:         <h3>End Screen</h3>
190:         <figure>
191:             <img src="screenshots/roguelike-end-screen.png" alt="Godot roguelike boss floor or end screen">
192:             <figcaption>Final floor and end-screen flow for victory or game over.</figcaption>
193:         </figure>
194:         <p>
195:             <a href="../projects.html">Back to Other Projects</a>
196:         </p>
197:     </section>
198: 
199: 
200: </body>
201: </html>
````

## File: old-site/projects/RESTful-AJAX-JSON-PHP-MySQL.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>RESTful Student Contacts Service - CIS 266</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>RESTful Student Contacts Service</h1>
 29: 
 30:         <p>
 31:             The RESTful Student Contacts Service is a PHP/MySQL web service project built for
 32:             CIS 266. The project demonstrates how a server-side PHP application can connect to
 33:             a MySQL database, retrieve student contact records, encode the results as JSON, and
 34:             make that data available to client-side pages through REST-style endpoints.
 35:         </p>
 36: 
 37:         <p>
 38:             The application includes both service-provider files and service-client files. The
 39:             provider side handles database access and JSON output, while the client side uses
 40:             jQuery AJAX requests to display all records or retrieve one selected record by
 41:             contact ID. The project also includes basic tester pages for directly testing the
 42:             API endpoints in the browser.
 43:         </p>
 44: 
 45:         <h2>Technologies Used</h2>
 46: 
 47:         <ul>
 48:             <li>PHP</li>
 49:             <li>MySQL</li>
 50:             <li>phpMyAdmin SQL export</li>
 51:             <li>HTML</li>
 52:             <li>JavaScript</li>
 53:             <li>jQuery AJAX</li>
 54:             <li>JSON</li>
 55:             <li>Localhost / WAMP-style development environment</li>
 56:         </ul>
 57: 
 58:         <h2>Features</h2>
 59: 
 60:         <ul>
 61:             <li>Connects to a MySQL database named <code>students</code></li>
 62:             <li>Uses a reusable PHP database access class for database operations</li>
 63:             <li>Displays all contact records from the student contacts table</li>
 64:             <li>Retrieves a single contact record by <code>contact_id</code></li>
 65:             <li>Returns API responses as JSON using <code>json_encode()</code></li>
 66:             <li>Includes API tester pages for directly checking service output</li>
 67:             <li>Includes client pages that consume the APIs with jQuery AJAX requests</li>
 68:             <li>Displays returned JSON data dynamically in the browser</li>
 69:             <li>Handles missing or invalid contact IDs with JSON error messages</li>
 70:             <li>Includes a SQL script for creating and populating the contacts table</li>
 71:         </ul>
 72: 
 73:         <h2>Code Sample</h2>
 74: 
 75:         <p>
 76:             This sample shows the PHP API endpoint used to retrieve one student contact record.
 77:             The script reads the <code>contact_id</code> value from the query string, checks that
 78:             the value was provided, queries the database through the database access class, and
 79:             returns either the matching record or an error message as JSON.
 80:         </p>
 81: 
 82:         <pre><code class="language-php">&lt;?php
 83: include_once("class_lib/StrJDB_Access.php");
 84: 
 85: $DB_Access = new StrJDB_Access();
 86: $table = "strj_unit2_ex1_contacts";
 87: 
 88: $contact_id = $_GET['contact_id'] ?? "";
 89: 
 90: if ($contact_id === "") {
 91:     print(json_encode(array("error" =&gt; "contact_id parameter is required")));
 92:     exit;
 93: }
 94: 
 95: $DB_Result = $DB_Access-&gt;selectOne($table, $contact_id);
 96: 
 97: if ($DB_Result &amp;&amp; $row = $DB_Result-&gt;fetch_assoc()) {
 98:     print(json_encode($row));
 99: } else {
100:     print(json_encode(array("error" =&gt; "Record not found")));
101: }
102: ?&gt;</code></pre>
103: 
104:         <p>
105:             This endpoint represents the main service pattern used in the project: receive a
106:             request parameter, call a database method, convert the result to JSON, and return
107:             that JSON response to a browser-based client.
108:         </p>
109: 
110:         <h2>App Screen Captures</h2>
111: 
112:         <h3>Home / Project Links Page</h3>
113:         <figure>
114:             <img src="screenshots/RESTful-AJAX-home.png" alt="RESTful Student Contacts project home page">
115:             <figcaption>Project home page with links to the service provider and client test pages.</figcaption>
116:         </figure>
117: 
118:         <h3>Display All Records Client</h3>
119:         <figure>
120:             <img src="screenshots/RESTful-AJAX-display-all.png" alt="Display all student contact records client page">
121:             <figcaption>Client page displaying all student contact records returned from the API.</figcaption>
122:         </figure>
123: 
124:         <h3>Display One Record Client</h3>
125:         <figure>
126:             <img src="screenshots/RESTful-AJAX-display-one.png" alt="Display one student contact record client page">
127:             <figcaption>Client page retrieving one student contact record by contact ID.</figcaption>
128:         </figure>
129: 
130:         <p>
131:             <a href="../cis266.html">Back to CIS 266 Projects</a>
132:         </p>
133:     </section>
134: 
135: 
136: </body>
137: </html>
````

## File: old-site/projects/simple-forum.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>Simple Forum Application - CIS 241</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26:     <section class="project-documentation">
 27:     <h1>Simple Forum Application</h1>
 28: 
 29:     <p>
 30:         The Simple Forum Application is a dynamic PHP/MySQL forum site built for CIS 241.
 31:         The project demonstrates a database-backed web application where users can register,
 32:         log in, browse forum categories, create posts, edit posts, and delete posts. The
 33:         application uses PHP for server-side logic, MySQL/MariaDB for persistent data storage,
 34:         PDO for database access, and Bootstrap for basic page styling.
 35:     </p>
 36: 
 37:     <p>
 38:         This project is externally hosted because GitHub Pages only supports static pages and
 39:         does not run PHP or MySQL. The hosted version demonstrates the actual working database
 40:         functionality required for the portfolio rubric.
 41:     </p>
 42: 
 43:     <h2>Features</h2>
 44: 
 45:     <ul>
 46:         <li>User registration with username, email, and password fields</li>
 47:         <li>Secure password hashing using PHP's <code>password_hash()</code> function</li>
 48:         <li>User login validation using <code>password_verify()</code></li>
 49:         <li>Session-based login and logout functionality</li>
 50:         <li>Optional "Remember Me" login token stored in the database</li>
 51:         <li>Forum category listing pulled from the database</li>
 52:         <li>Category-based post viewing</li>
 53:         <li>Create, edit, and delete forum posts</li>
 54:         <li>MySQL database structure for users, categories, and posts</li>
 55:         <li>PDO prepared statements for database queries</li>
 56:         <li>Bootstrap-based responsive layout</li>
 57:         <li>Dynamic navigation that changes depending on whether the user is logged in</li>
 58:     </ul>
 59: 
 60:     <h2>Code Sample</h2>
 61: 
 62:     <p>
 63:         This sample shows the post update function from the project. It uses a prepared SQL
 64:         statement with bound values to safely update a forum post in the database.
 65:     </p>
 66: 
 67:     <pre><code class="language-php">function update_post($id, $title, $content) {
 68:     global $db;
 69: 
 70:     $query = 'UPDATE posts
 71:               SET title = :title,
 72:                   content = :content
 73:               WHERE id = :id';
 74: 
 75:     $statement = $db-&gt;prepare($query);
 76:     $statement-&gt;bindValue(':title', $title);
 77:     $statement-&gt;bindValue(':content', $content);
 78:     $statement-&gt;bindValue(':id', $id, PDO::PARAM_INT);
 79: 
 80:     $success = $statement-&gt;execute();
 81:     $statement-&gt;closeCursor();
 82: 
 83:     return $success;
 84: }</code></pre>
 85: 
 86:     <p>
 87:         This function represents the main database pattern used throughout the application:
 88:         prepare the query, bind user-provided values, execute the statement, and close the cursor.
 89:     </p>
 90: 
 91:     <h2>App Screen Captures</h2>
 92: 
 93:     <h3>Home / Forum Categories Page</h3>
 94:     <figure>
 95:         <img src="screenshots/simple-forum-home.png" alt="Simple Forum home page showing forum categories">
 96:         <figcaption>Forum categories loaded from the database.</figcaption>
 97:     </figure>
 98: 
 99:     <h3>Post Creation Page</h3>
100:     <figure>
101:         <img src="screenshots/simple-forum-create-post.png" alt="Simple Forum post creation page with form fields for title and content">
102:         <figcaption>Creating a new forum post.</figcaption>
103:     </figure>
104: 
105:     <h3>Viewing Posts</h3>
106:     <figure>
107:         <img src="screenshots/simple-forum-view-post.png" alt="Simple Forum posts page">
108:         <figcaption>Posts displayed for a selected forum category.</figcaption>
109:     </figure>
110: 
111:     <h2>Demo</h2>
112: 
113:     <p>
114:         <a href="https://cis241simpleforum.ct.ws/index.php" target="_blank" rel="noopener noreferrer">
115:             Try the app live here!
116:         </a>
117:         Create an account, log in, and explore the forum functionality.
118:     </p>
119: 
120:     <p>
121:         <a href="../cis241.html">Back to CIS 241 Projects</a>
122:     </p>
123: </section>
124: 
125: 
126: </body>
127: </html>
````

## File: old-site/projects/sportspro.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>SportsPro Technical Support - CIS 296</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>SportsPro Technical Support</h1>
 29: 
 30:         <p>
 31:             SportsPro Technical Support is an ASP.NET Core MVC application built for CIS 296.
 32:             The project demonstrates a database-backed support management system where users
 33:             can maintain product, customer, technician, and incident records through standard
 34:             MVC list, add, edit, and delete workflows.
 35:         </p>
 36: 
 37:         <p>
 38:             The application uses Entity Framework Core with a SQL Server LocalDB database.
 39:             It includes model classes, controllers, Razor views, validation attributes,
 40:             database migrations, seeded sample data, and Bootstrap-based layout styling.
 41:             A more advanced part of the project is the technician incident workflow, where
 42:             the selected technician is stored in session and then used to display only that
 43:             technician's open incidents.
 44:         </p>
 45: 
 46:         <h2>Technologies Used</h2>
 47: 
 48:         <ul>
 49:             <li>C#</li>
 50:             <li>ASP.NET Core MVC</li>
 51:             <li>.NET 6</li>
 52:             <li>Entity Framework Core 6.0.10</li>
 53:             <li>SQL Server LocalDB</li>
 54:             <li>Razor views</li>
 55:             <li>Bootstrap</li>
 56:             <li>Model validation with data annotations</li>
 57:             <li>Entity Framework migrations</li>
 58:             <li>Session state</li>
 59:             <li>Dependency injection</li>
 60:         </ul>
 61: 
 62:         <h2>Features</h2>
 63: 
 64:         <ul>
 65:             <li>Home and About pages using MVC routing</li>
 66:             <li>Product management with list, add, edit, and delete functionality</li>
 67:             <li>Technician management with list, add, edit, and delete functionality</li>
 68:             <li>Customer management with country dropdown selection</li>
 69:             <li>Incident management with customer, product, and technician relationships</li>
 70:             <li>Incident filtering by all, open, or unassigned status</li>
 71:             <li>Incident add/edit form backed by a view model for dropdown data</li>
 72:             <li>Technician selection page for technician-specific incident work</li>
 73:             <li>Session-based storage of the selected technician</li>
 74:             <li>Technician-specific incident list showing open incidents assigned to that technician</li>
 75:             <li>Technician incident edit page for updating assigned incidents</li>
 76:             <li>Entity Framework navigation properties and eager loading with <code>Include()</code></li>
 77:             <li>Data annotation validation for required fields, string lengths, ranges, and dates</li>
 78:             <li>Initial migration that creates and seeds countries, products, technicians, customers, and incidents</li>
 79:             <li>Bootstrap layout and shared Razor layout page</li>
 80:         </ul>
 81: 
 82:         <h2>Code Sample</h2>
 83: 
 84:         <p>
 85:             This sample shows the incident list logic from the project. The controller builds
 86:             an Entity Framework query that includes related customer, product, and technician
 87:             data, then filters the incident list depending on the selected status.
 88:         </p>
 89: 
 90:         <pre><code class="language-csharp">[HttpGet]
 91: [Route("Incidents")]
 92: public ViewResult List(IncidentListViewModel model)
 93: {
 94:     IQueryable&lt;Incident&gt; query = context.Incidents
 95:         .Include(i =&gt; i.Customer)
 96:         .Include(i =&gt; i.Product)
 97:         .Include(i =&gt; i.Technician);
 98: 
 99:     if (model.IncidentStatus == "unassigned")
100:     {
101:         query = query.Where(i =&gt; i.TechnicianID == -1);
102:     }
103:     else if (model.IncidentStatus == "open")
104:     {
105:         query = query.Where(i =&gt; i.DateClosed == null);
106:     }
107: 
108:     model.Incidents = query.OrderBy(i =&gt; i.DateOpened).ToList();
109: 
110:     return View(model);
111: }</code></pre>
112: 
113:         <p>
114:             This code represents one of the main MVC patterns used in the application:
115:             query the database through the injected context, include related records needed
116:             by the view, apply filtering logic, store the result in a view model, and return
117:             that model to a Razor view.
118:         </p>
119: 
120:         <h2>App Screen Captures</h2>
121: 
122:         <h3>SportsPro Home Page</h3>
123:         <figure>
124:             <img src="screenshots/sportspro-home.png" alt="SportsPro home page">
125:             <figcaption>Home page for the SportsPro technical support application.</figcaption>
126:         </figure>
127:         
128:         <h3>Incident List and Filters</h3>
129:         <figure>
130:             <img src="screenshots/sportspro-incidents.png" alt="SportsPro incident list with filters">
131:             <figcaption>Incident list with related customer, product, technician, and status information.</figcaption>
132:         </figure>
133: 
134:         <h3>Technician Incident Workflow</h3>
135:         <figure>
136:             <img src="screenshots/sportspro-technician-incidents.png" alt="SportsPro technician incident workflow">
137:             <figcaption>Technician-specific workflow for selecting a technician and updating assigned incidents.</figcaption>
138:         </figure>
139: 
140:         <p>
141:             <a href="../cis296.html">Back to CIS 296 Projects</a>
142:         </p>
143:     </section>
144: 
145: 
146: </body>
147: </html>
````

## File: old-site/projects/switcher.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>Display Switcher CLI - Project Documentation</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>Display Switcher CLI</h1>
 29: 
 30:         <p>
 31:             Display Switcher CLI is a Go command-line application created to quickly switch
 32:             between different Windows monitor and workspace setups. The tool reads named
 33:             profiles from a JSON configuration file and applies the actions assigned to each
 34:             profile, such as loading a saved monitor configuration, disabling displays,
 35:             launching desktop applications, or opening useful URLs.
 36:         </p>
 37: 
 38:         <p>
 39:             The project was built as a practical automation tool for managing different
 40:             computer setups. For example, one profile can restore a full desk layout with
 41:             multiple monitors, while another profile can simplify the display setup for use
 42:             from bed. Additional profiles can launch school-related apps, gaming apps, or
 43:             frequently used websites after the display layout is applied.
 44:         </p>
 45: 
 46:         <h2>Technologies Used</h2>
 47: 
 48:         <ul>
 49:             <li>Go</li>
 50:             <li>Cobra CLI library</li>
 51:             <li>JSON configuration</li>
 52:             <li>Windows command execution</li>
 53:             <li>NirSoft MultiMonitorTool</li>
 54:             <li>Saved monitor configuration files</li>
 55:             <li>Go modules</li>
 56:             <li>Windows executable build</li>
 57:         </ul>
 58: 
 59:         <h2>Features</h2>
 60: 
 61:         <ul>
 62:             <li>Provides a command-line interface named <code>displayswitcher</code></li>
 63:             <li>Uses Cobra subcommands for organizing CLI behavior</li>
 64:             <li>Loads profile data from <code>config.json</code></li>
 65:             <li>Supports a global <code>--config</code> flag for using a custom config file path</li>
 66:             <li>Lists all available profiles with the <code>list</code> command</li>
 67:             <li>Shows the actions assigned to a profile with the <code>show</code> command</li>
 68:             <li>Applies a selected profile with the <code>apply</code> command</li>
 69:             <li>Supports a <code>--dry-run</code> flag to preview actions without executing them</li>
 70:             <li>Loads saved display layouts using <code>MultiMonitorTool.exe</code></li>
 71:             <li>Can disable specific displays before applying a monitor profile</li>
 72:             <li>Can launch desktop applications as part of a workspace profile</li>
 73:             <li>Can open URLs in the default browser</li>
 74:             <li>Includes separate profiles for bed, desk, school, and gaming workflows</li>
 75:             <li>Includes saved monitor configuration files for different display layouts</li>
 76:         </ul>
 77: 
 78:         <h2>Code Sample</h2>
 79: 
 80:         <p>
 81:             This sample shows the configuration loading logic used by the CLI. The function
 82:             reads a JSON file, parses it into Go structs, and returns a usable configuration
 83:             object to the command files.
 84:         </p>
 85: 
 86:         <pre><code class="language-go">type Config struct {
 87:     Profiles map[string]Profile `json:"profiles"`
 88: }
 89: 
 90: type Profile struct {
 91:     Actions []Action `json:"actions"`
 92: }
 93: 
 94: type Action struct {
 95:     Type string `json:"type"`
 96:     Path string `json:"path,omitempty"`
 97: }
 98: 
 99: func Load(path string) (Config, error) {
100:     b, err := os.ReadFile(path)
101:     if err != nil {
102:         return Config{}, fmt.Errorf("read %q: %w", path, err)
103:     }
104: 
105:     var cfg Config
106:     if err := json.Unmarshal(b, &amp;cfg); err != nil {
107:         return Config{}, fmt.Errorf("parse %q: %w", path, err)
108:     }
109: 
110:     if cfg.Profiles == nil {
111:         cfg.Profiles = map[string]Profile{}
112:     }
113: 
114:     return cfg, nil
115: }</code></pre>
116: 
117:         <p>
118:             This code represents the foundation of the tool. The CLI commands all depend on
119:             the same configuration structure, allowing the application to treat each profile
120:             as a named list of actions that can be listed, inspected, or executed.
121:         </p>
122: 
123:         <h2>App Screen Captures</h2>
124: 
125:         <h3>Available Profiles Command</h3>
126:         <figure>
127:             <img src="screenshots/display-switcher-list.png" alt="Display Switcher CLI list command output">
128:             <figcaption>Output showing available display and workspace profiles.</figcaption>
129:         </figure>
130: 
131:         <h3>Profile Details Command</h3>
132:         <figure>
133:             <img src="screenshots/display-switcher-show.png" alt="Display Switcher CLI show command output">
134:             <figcaption>Output showing the actions assigned to a selected profile.</figcaption>
135:         </figure>
136: 
137:         <h3>Apply Profile Command</h3>
138:         <figure>
139:             <img src="screenshots/display-switcher-apply.png" alt="Display Switcher CLI apply command output">
140:             <figcaption>Applying a saved display or workspace profile from the terminal.</figcaption>
141:         </figure>
142: 
143:         <h2>Demo</h2>
144: 
145:         <p>
146:             <a href="https://stc.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=0107982d-c1fc-4c68-8597-b40701357aba" rel="noopener noreferrer">
147:                 View the project demo here!
148:             </a>
149:             The demo video shows the CLI tool in action, applying different display and workspace. I cut out the section going through code, because I expose my montior ID.
150:         </p>
151: 
152:         <p>
153:             <a href="../projects.html">Back to Other Projects</a>
154:         </p>
155:     </section>
156: 
157: 
158: </body>
159: </html>
````

## File: old-site/projects/voting-system.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>Real-Time Voting System - CIS 266</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>Real-Time Voting System</h1>
 29: 
 30:         <p>
 31:             The Real-Time Voting System is a Node.js and Socket.IO project built for CIS 266.
 32:             The application allows users to vote for their favorite programming language and
 33:             see the poll results update instantly in the browser. Instead of requiring a page
 34:             refresh, the server broadcasts updated vote totals to every connected client in
 35:             real time.
 36:         </p>
 37: 
 38:         <p>
 39:             The project separates the client and server logic into different folders. The
 40:             client side contains the HTML page, CSS styling, and browser JavaScript used to
 41:             send votes and render result bars. The server side uses Node.js to serve the static
 42:             files, maintain the vote state, listen for Socket.IO events, and push updated
 43:             results back to all connected users.
 44:         </p>
 45: 
 46:         <h2>Technologies Used</h2>
 47: 
 48:         <ul>
 49:             <li>Node.js</li>
 50:             <li>Socket.IO</li>
 51:             <li>JavaScript</li>
 52:             <li>HTML</li>
 53:             <li>CSS</li>
 54:             <li>HTTP server module</li>
 55:             <li>File system module</li>
 56:             <li>Path module</li>
 57:             <li>npm package management</li>
 58:             <li>Localhost development server</li>
 59:         </ul>
 60: 
 61:         <h2>Features</h2>
 62: 
 63:         <ul>
 64:             <li>Allows users to vote for JavaScript, Python, or C#</li>
 65:             <li>Sends votes from the browser to the server using Socket.IO events</li>
 66:             <li>Stores live vote counts on the Node.js server</li>
 67:             <li>Broadcasts updated results to all connected clients</li>
 68:             <li>Updates the browser interface instantly without refreshing the page</li>
 69:             <li>Displays vote counts beside each poll option</li>
 70:             <li>Calculates result percentages based on the current vote total</li>
 71:             <li>Displays animated horizontal result bars</li>
 72:             <li>Includes a reset button that clears all vote totals</li>
 73:             <li>Supports testing with multiple browser tabs to simulate multiple users</li>
 74:             <li>Serves the client HTML, JavaScript, and CSS files from the Node.js server</li>
 75:         </ul>
 76: 
 77:         <h2>Code Sample</h2>
 78: 
 79:         <p>
 80:             This sample shows the Socket.IO server logic for the voting system. When a user
 81:             connects, the server sends the current vote totals. When a vote or reset event is
 82:             received, the server updates the vote state and broadcasts the new results to every
 83:             connected client.
 84:         </p>
 85: 
 86:         <pre><code class="language-javascript">// Socket.IO setup
 87: const io = require('socket.io')(server, {
 88:     cors: { origin: '*' }
 89: });
 90: 
 91: // Voting state
 92: let votes = {
 93:     JavaScript: 0,
 94:     Python: 0,
 95:     'C#': 0
 96: };
 97: 
 98: // Handle socket connections
 99: io.on('connection', (socket) =&gt; {
100:     console.log('User connected');
101: 
102:     // Send current results immediately
103:     socket.emit('updateResults', votes);
104: 
105:     // Handle vote
106:     socket.on('vote', (option) =&gt; {
107:         if (votes[option] !== undefined) {
108:             votes[option]++;
109:             io.emit('updateResults', votes);
110:         }
111:     });
112: 
113:     // Reset poll
114:     socket.on('reset', () =&gt; {
115:         for (let key in votes) {
116:             votes[key] = 0;
117:         }
118:         io.emit('updateResults', votes);
119:     });
120: });</code></pre>
121: 
122:         <p>
123:             This code represents the main real-time communication pattern used in the project:
124:             clients emit events to the server, the server updates shared application state, and
125:             Socket.IO broadcasts the new state back to all connected clients.
126:         </p>
127: 
128:         <h2>App Screen Captures</h2>
129: 
130:         <h3>Voting Page with Multiple Clients</h3>
131:         <figure>
132:             <img src="screenshots/realtime-voting-home.png" alt="Real-time voting application page">
133:             <figcaption>Voting interface with programming language options.</figcaption>
134:         </figure>
135: 
136:         <h3>Live Results</h3>
137:         <figure>
138:             <img src="screenshots/realtime-voting-results.png" alt="Live voting results with result bars">
139:             <figcaption>Live result bars updating after users vote. Both clients update in real time, with no browser refresh.</figcaption>
140:         </figure>
141: 
142:         <h3>Demo Video</h3>
143:         <figure>
144:             click <a href="https://stc.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=9219fb79-5cec-4967-9a82-b43b0000def3">here</a> to view the demo video
145:         </figure>
146: 
147:         <h2>Presentation Slides</h2>
148:         <figure>
149:             <img src="screenshots/Slide1.PNG">
150:             <img src="screenshots/Slide2.PNG">
151:             <img src="screenshots/Slide3.PNG">
152:             <img src="screenshots/Slide4.PNG">
153:             <img src="screenshots/Slide5.PNG">
154:             <img src="screenshots/Slide6.PNG">
155:         </figure>
156: 
157:         <p>
158:             <a href="../cis266.html">Back to CIS 266 Projects</a>
159:         </p>
160:     </section>
161: 
162: 
163: </body>
164: </html>
````

## File: old-site/projects/wcf.html
````html
  1: <!DOCTYPE html>
  2: <html lang="en">
  3: <head>
  4:     <meta charset="UTF-8">
  5:     <meta name="viewport" content="width=device-width, initial-scale=1.0">
  6:     <link rel="stylesheet" href="../css/styles.css">
  7:     <title>Library Record WCF Service - CIS 266</title>
  8: </head>
  9: <body>
 10:     <nav>
 11:         <a href="../index.html" class="brand">Jared Street</a>
 12:         <ul>
 13:             <li><a href="../index.html">Home</a></li>
 14:             <li><a href="../documents/JaredStreetResume.pdf">Resume</a></li>
 15:             <li><a href="../CIS_Syllabi.html">CIS Syllabi</a></li>
 16:             <li><a href="../cis241.html">CIS 241 Projects</a></li>
 17:             <li><a href="../cis266.html">CIS 266 Web Services</a></li>
 18:             <li><a href="../cis296.html">CIS 296 C# Projects</a></li>
 19:             <li>
 20:                 <a href="http://catalog.southeasttech.edu/preview_program.php?catoid=17&poid=2004&hl=%22programming%22">
 21:                     STI CIS Curriculum
 22:                 </a>
 23:             </li>
 24:         </ul>
 25:     </nav>
 26: 
 27:     <section class="project-documentation">
 28:         <h1>Library Record WCF Service</h1>
 29: 
 30:         <p>
 31:             The Library Record WCF Service is a C# web service project built for CIS 266.
 32:             The project demonstrates how to define a WCF service contract, expose book
 33:             management operations, and consume those operations from a separate console
 34:             client application.
 35:         </p>
 36: 
 37:         <p>
 38:             The solution contains two main projects. The <code>CampusBookingSystemJS</code>
 39:             project hosts the WCF service and defines the service contract, data contract,
 40:             and service implementation. The <code>LibraryConsole</code> project connects to
 41:             the service through a generated service reference and provides a menu-driven
 42:             console interface for testing the library record operations.
 43:         </p>
 44: 
 45:         <h2>Technologies Used</h2>
 46: 
 47:         <ul>
 48:             <li>C#</li>
 49:             <li>.NET Framework 4.8</li>
 50:             <li>Windows Communication Foundation, or WCF</li>
 51:             <li>Visual Studio 2022</li>
 52:             <li>IIS Express / local WCF hosting</li>
 53:             <li>Service contracts and operation contracts</li>
 54:             <li>Data contracts and data members</li>
 55:             <li>Connected service references</li>
 56:             <li>Console application client</li>
 57:             <li>In-memory list storage using <code>List&lt;Book&gt;</code></li>
 58:         </ul>
 59: 
 60:         <h2>Features</h2>
 61: 
 62:         <ul>
 63:             <li>Defines a WCF service contract with book management operations</li>
 64:             <li>Uses a <code>Book</code> data contract with book ID, title, author, ISBN, and availability fields</li>
 65:             <li>Adds new book records through the service</li>
 66:             <li>Updates existing book title, author, and ISBN data</li>
 67:             <li>Deletes books by book ID</li>
 68:             <li>Retrieves one book by book ID</li>
 69:             <li>Lists all books currently stored in the service</li>
 70:             <li>Searches books by title</li>
 71:             <li>Searches books by author</li>
 72:             <li>Searches for one book by ISBN</li>
 73:             <li>Checks whether a book is available</li>
 74:             <li>Checks out a book by changing its availability status</li>
 75:             <li>Returns a checked-out book by marking it available again</li>
 76:             <li>Uses WCF fault exceptions to report invalid input and missing records</li>
 77:             <li>Provides a menu-driven console client for testing service operations</li>
 78:         </ul>
 79: 
 80:         <h2>Code Sample</h2>
 81: 
 82:         <p>
 83:             This sample shows the service contract and the <code>Book</code> data contract.
 84:             The service contract declares the operations that the console client can call,
 85:             while the data contract defines the book object passed between the client and
 86:             the WCF service.
 87:         </p>
 88: 
 89:         <pre><code class="language-csharp">[ServiceContract]
 90: public interface IService1
 91: {
 92:     [OperationContract]
 93:     void AddBook(Book book);
 94: 
 95:     [OperationContract]
 96:     void UpdateBook(Book book);
 97: 
 98:     [OperationContract]
 99:     void DeleteBook(int bookID);
100: 
101:     [OperationContract]
102:     Book GetBook(int bookID);
103: 
104:     [OperationContract]
105:     List&lt;Book&gt; GetAllBooks();
106: 
107:     [OperationContract]
108:     List&lt;Book&gt; SearchByTitle(string title);
109: 
110:     [OperationContract]
111:     List&lt;Book&gt; SearchByAuthor(string author);
112: 
113:     [OperationContract]
114:     Book SearchByISBN(string isbn);
115: 
116:     [OperationContract]
117:     bool CheckBookAvailability(int bookID);
118: 
119:     [OperationContract]
120:     void CheckOutBook(int bookID);
121: 
122:     [OperationContract]
123:     void ReturnBook(int bookID);
124: }
125: 
126: [DataContract]
127: public class Book
128: {
129:     [DataMember]
130:     public int BookID { get; set; }
131: 
132:     [DataMember]
133:     public string Title { get; set; }
134: 
135:     [DataMember]
136:     public string Author { get; set; }
137: 
138:     [DataMember]
139:     public string ISBN { get; set; }
140: 
141:     [DataMember]
142:     public bool IsAvailable { get; set; }
143: }</code></pre>
144: 
145:         <p>
146:             This code represents the core WCF structure of the project: the service contract
147:             lists the operations exposed by the service, and the data contract defines the
148:             data shape shared between the WCF service and the console client.
149:         </p>
150: 
151:         <h2>App Screen Captures</h2>
152: 
153:         <h3>WCF Service Running in Browser</h3>
154:         <figure>
155:             <img src="screenshots/library-wcf-service-browser.png" alt="Library WCF service running in browser">
156:             <figcaption>Local WCF service page showing that the service is running.</figcaption>
157:         </figure>
158: 
159:         <h3>Console Application Menu</h3>
160:         <figure>
161:             <img src="screenshots/library-console-menu.png" alt="Library console application menu">
162:             <figcaption>Menu-driven console client used to call the WCF service operations.</figcaption>
163:         </figure>
164: 
165:         <h3>Book Operation Output</h3>
166:         <figure>
167:             <img src="screenshots/library-console-output.png" alt="Library console output showing book records">
168:             <figcaption>Console output showing book records returned from the WCF service.</figcaption>
169:         </figure>
170: 
171:         <p>
172:             <a href="../cis266.html">Back to CIS 266 Projects</a>
173:         </p>
174:     </section>
175: 
176: 
177: </body>
178: </html>
````

## File: package.json
````json
 1: {
 2:   "name": "galactic-giant",
 3:   "type": "module",
 4:   "version": "0.0.1",
 5:   "engines": {
 6:     "node": ">=22.12.0"
 7:   },
 8:   "scripts": {
 9:     "dev": "astro dev",
10:     "build": "astro build",
11:     "preview": "astro preview",
12:     "astro": "astro"
13:   },
14:   "dependencies": {
15:     "astro": "^6.4.6"
16:   }
17: }
````

## File: public/favicon.svg
````xml
1: <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 128 128">
2:     <path d="M50.4 78.5a75.1 75.1 0 0 0-28.5 6.9l24.2-65.7c.7-2 1.9-3.2 3.4-3.2h29c1.5 0 2.7 1.2 3.4 3.2l24.2 65.7s-11.6-7-28.5-7L67 45.5c-.4-1.7-1.6-2.8-2.9-2.8-1.3 0-2.5 1.1-2.9 2.7L50.4 78.5Zm-1.1 28.2Zm-4.2-20.2c-2 6.6-.6 15.8 4.2 20.2a17.5 17.5 0 0 1 .2-.7 5.5 5.5 0 0 1 5.7-4.5c2.8.1 4.3 1.5 4.7 4.7.2 1.1.2 2.3.2 3.5v.4c0 2.7.7 5.2 2.2 7.4a13 13 0 0 0 5.7 4.9v-.3l-.2-.3c-1.8-5.6-.5-9.5 4.4-12.8l1.5-1a73 73 0 0 0 3.2-2.2 16 16 0 0 0 6.8-11.4c.3-2 .1-4-.6-6l-.8.6-1.6 1a37 37 0 0 1-22.4 2.7c-5-.7-9.7-2-13.2-6.2Z" />
3:     <style>
4:         path { fill: #000; }
5:         @media (prefers-color-scheme: dark) {
6:             path { fill: #FFF; }
7:         }
8:     </style>
9: </svg>
````

## File: README.md
````markdown
 1: # Astro Starter Kit: Minimal
 2: 
 3: ```sh
 4: npm create astro@latest -- --template minimal
 5: ```
 6: 
 7: > 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!
 8: 
 9: ## 🚀 Project Structure
10: 
11: Inside of your Astro project, you'll see the following folders and files:
12: 
13: ```text
14: /
15: ├── public/
16: ├── src/
17: │   └── pages/
18: │       └── index.astro
19: └── package.json
20: ```
21: 
22: Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.
23: 
24: There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.
25: 
26: Any static assets, like images, can be placed in the `public/` directory.
27: 
28: ## 🧞 Commands
29: 
30: All commands are run from the root of the project, from a terminal:
31: 
32: | Command                   | Action                                           |
33: | :------------------------ | :----------------------------------------------- |
34: | `npm install`             | Installs dependencies                            |
35: | `npm run dev`             | Starts local dev server at `localhost:4321`      |
36: | `npm run build`           | Build your production site to `./dist/`          |
37: | `npm run preview`         | Preview your build locally, before deploying     |
38: | `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
39: | `npm run astro -- --help` | Get help using the Astro CLI                     |
40: 
41: ## 👀 Want to learn more?
42: 
43: Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
````

## File: src/components/Footer.astro
````astro
1: <footer class="site-footer">
2:   <p>&copy; 2026 Jared Street. Built with Astro.</p>
3: 
4:   <div class="footer-links">
5:     <a href="/documents/JaredStreetResume.pdf">Resume</a>
6:     <a href="https://github.com/OhStreet" target="_blank" rel="noopener noreferrer">GitHub</a>
7:     <a href="/#contact">Contact</a>
8:   </div>
9: </footer>
````

## File: src/components/Nav.astro
````astro
 1: ---
 2: const currentPath = Astro.url.pathname;
 3: 
 4: const isActive = (path: string) => {
 5:   if (path === "/") {
 6:     return currentPath === "/";
 7:   }
 8: 
 9:   return currentPath.startsWith(path);
10: };
11: ---
12: 
13: <header class="site-header">
14:   <nav class="nav-container" aria-label="Main navigation">
15:     <a class="brand" href="/">
16:       Jared Street
17:     </a>
18: 
19:     <ul class="nav-links">
20:       <li>
21:         <a href="/" class={isActive("/") ? "active" : ""}>Home</a>
22:       </li>
23:       <li>
24:         <a href="/projects/" class={isActive("/projects") ? "active" : ""}>Projects</a>
25:       </li>
26:       <li>
27:         <a href="/#skills">Skills</a>
28:       </li>
29:       <li>
30:         <a href="/#contact">Contact</a>
31:       </li>
32:       <li>
33:         <a href="/documents/JaredStreetResume.pdf">Resume</a>
34:       </li>
35:       <li>
36:         <a href="https://github.com/OhStreet" target="_blank" rel="noopener noreferrer">
37:           GitHub
38:         </a>
39:       </li>
40:       <!-- Add LinkedIn later -->
41:     </ul>
42:   </nav>
43: </header>
````

## File: src/layouts/BaseLayout.astro
````astro
 1: ---
 2: import Nav from "../components/Nav.astro";
 3: import Footer from "../components/Footer.astro";
 4: import "../styles/global.css";
 5: 
 6: interface Props {
 7:   title?: string;
 8:   description?: string;
 9: }
10: 
11: const {
12:   title = "Jared Street | Entry-Level Software Developer",
13:   description = "Portfolio for Jared Street, an entry-level software developer focused on web, database, and application projects.",
14: } = Astro.props;
15: ---
16: 
17: <!doctype html>
18: <html lang="en">
19:   <head>
20:     <meta charset="UTF-8" />
21:     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
22:     <meta name="description" content={description} />
23:     <title>{title}</title>
24:   </head>
25: 
26:   <body>
27:     <Nav />
28: 
29:     <main class="site-main">
30:       <slot />
31:     </main>
32: 
33:     <Footer />
34:   </body>
35: </html>
````

## File: src/styles/global.css
````css
  1: :root {
  2:   --bg: #0a1020;
  3:   --bg-soft: #111827;
  4:   --panel: #192235;
  5:   --border: #334155;
  6:   --text: #f1f5f9;
  7:   --muted: #a8b3c7;
  8:   --accent: #fb7185;
  9:   --accent-soft: rgba(251, 113, 133, 0.13);
 10:   --link: #fda4af;
 11:   --link-hover: #ffe4e6;
 12: 
 13:   --max-width: 1440px;
 14:   --radius: 16px;
 15: }
 16: 
 17: * {
 18:   box-sizing: border-box;
 19: }
 20: 
 21: html {
 22:   scroll-behavior: smooth;
 23: }
 24: 
 25: body {
 26:   margin: 0;
 27:   min-height: 100vh;
 28:   background:
 29:     radial-gradient(circle at top left, rgba(96, 165, 250, 0.12), transparent 32rem),
 30:     var(--bg);
 31:   color: var(--text);
 32:   font-family: Arial, Helvetica, sans-serif;
 33:   line-height: 1.6;
 34: }
 35: 
 36: h1,
 37: h2,
 38: h3 {
 39:   line-height: 1.1;
 40:   letter-spacing: -0.02em;
 41: }
 42: 
 43: h2 {
 44:   font-size: clamp(2rem, 4vw, 3rem);
 45: }
 46: 
 47: /* p {
 48:   max-width: 75ch;
 49: } */
 50: 
 51: a {
 52:   color: var(--link);
 53:   text-decoration: none;
 54: }
 55: 
 56: a:hover {
 57:   color: var(--link-hover);
 58: }
 59: 
 60: img {
 61:   max-width: 100%;
 62:   height: auto;
 63:   display: block;
 64: }
 65: 
 66: .site-header {
 67:   position: sticky;
 68:   top: 0;
 69:   z-index: 10;
 70:   background: rgba(15, 23, 42, 0.92);
 71:   backdrop-filter: blur(12px);
 72:   border-bottom: 1px solid var(--border);
 73: }
 74: 
 75: .nav-container {
 76:   max-width: var(--max-width);
 77:   margin: 0 auto;
 78:   padding: 1rem 1.5rem;
 79:   display: flex;
 80:   justify-content: space-between;
 81:   align-items: center;
 82:   gap: 2rem;
 83: }
 84: 
 85: .brand {
 86:   color: var(--text);
 87:   font-weight: 800;
 88:   font-size: 1.1rem;
 89:   letter-spacing: 0.02em;
 90: }
 91: 
 92: .nav-links {
 93:   list-style: none;
 94:   display: flex;
 95:   align-items: center;
 96:   gap: 1.25rem;
 97:   margin: 0;
 98:   padding: 0;
 99: }
100: 
101: .nav-links a {
102:   color: var(--muted);
103:   font-size: 0.95rem;
104:   font-weight: 600;
105: }
106: 
107: .nav-links a:hover,
108: .nav-links a.active {
109:   color: var(--accent);
110: }
111: 
112: .site-main {
113:   max-width: var(--max-width);
114:   margin: 0 auto;
115:   padding: 3rem 1.5rem;
116: }
117: 
118: section {
119:   margin-bottom: 4rem;
120: }
121: 
122: .section-card {
123:   background:
124:     linear-gradient(135deg, rgba(255, 255, 255, 0.035), transparent),
125:     rgba(17, 24, 39, 0.84);
126:   border: 1px solid var(--border);
127:   border-radius: var(--radius);
128:   padding: 2rem;
129:   box-shadow: 0 20px 60px rgba(0, 0, 0, 0.18);
130: }
131: 
132: .eyebrow {
133:   color: var(--accent);
134:   text-transform: uppercase;
135:   letter-spacing: 0.18em;
136:   font-size: 0.8rem;
137:   font-weight: 800;
138:   margin-bottom: 0.75rem;
139: }
140: 
141: .site-footer {
142:   border-top: 1px solid var(--border);
143:   background: var(--bg-soft);
144:   color: var(--muted);
145:   padding: 2rem 1.5rem;
146:   text-align: center;
147: }
148: 
149: .footer-links {
150:   margin-top: 0.75rem;
151:   display: flex;
152:   justify-content: center;
153:   gap: 1rem;
154:   flex-wrap: wrap;
155: }
156: 
157: .footer-links a {
158:   color: var(--muted);
159:   font-weight: 600;
160: }
161: 
162: .footer-links a:hover {
163:   color: var(--accent);
164: }
165: 
166: #hero h1 {
167:   font-size: clamp(2.5rem, 7vw, 5rem);
168:   line-height: 1;
169:   margin: 0 0 1rem;
170: }
171: 
172: #hero p:last-child {
173:   max-width: 720px;
174:   color: var(--muted);
175:   font-size: 1.1rem;
176: }
177: 
178: .button-row {
179:   display: flex;
180:   flex-wrap: wrap;
181:   gap: 1rem;
182:   margin-top: 1.5rem;
183: }
184: 
185: .button {
186:   display: inline-flex;
187:   align-items: center;
188:   justify-content: center;
189:   border-radius: 999px;
190:   padding: 0.75rem 1.1rem;
191:   margin-top: 1rem;
192:   font-weight: 700;
193:   border: 1px solid var(--border);
194:   transition: transform 160ms ease, border-color 160ms ease, background 160ms ease;
195: }
196: 
197: .button:hover {
198:   transform: translateY(-2px);
199: }
200: 
201: .button-primary {
202:   background: var(--accent);
203:   color: var(--bg);
204:   border-color: var(--accent);
205: }
206: 
207: .button-primary:hover {
208:   color: var(--bg);
209: }
210: 
211: .button-secondary {
212:   background: transparent;
213:   color: var(--text);
214: }
215: 
216: .button-secondary:hover {
217:   border-color: var(--accent);
218:   color: var(--accent);
219: }
220: 
221: .project-grid {
222:   display: grid;
223:   grid-template-columns: repeat(2, minmax(0, 1fr));
224:   gap: 1.25rem;
225:   margin-top: 1.5rem;
226: }
227: 
228: .project-card {
229:   background: rgba(17, 24, 39, 0.78);
230:   border: 1px solid var(--border);
231:   border-radius: var(--radius);
232:   padding: 1.5rem;
233:   transition: transform 160ms ease, border-color 160ms ease, box-shadow 160ms ease;
234: }
235: 
236: .project-card:hover {
237:   transform: translateY(-4px);
238:   border-color: var(--accent);
239:   box-shadow: 0 20px 45px rgba(0, 0, 0, 0.22);
240: }
241: 
242: .project-card h3 {
243:   margin-top: 0;
244:   margin-bottom: 0.5rem;
245: }
246: 
247: .project-card p {
248:   color: var(--muted);
249: }
250: 
251: .tech-list {
252:   display: flex;
253:   flex-wrap: wrap;
254:   gap: 0.5rem;
255:   margin-top: 1rem;
256: }
257: 
258: .tech-pill {
259:   border: 1px solid var(--border);
260:   border-radius: 999px;
261:   padding: 0.3rem 0.65rem;
262:   color: var(--muted);
263:   font-size: 0.85rem;
264: }
265: 
266: .page-hero {
267:   margin-bottom: 3rem;
268: }
269: 
270: .page-hero h1 {
271:   font-size: clamp(2.75rem, 7vw, 5rem);
272:   line-height: 1;
273:   margin: 0 0 1rem;
274: }
275: 
276: .page-hero p:last-child {
277:   max-width: 780px;
278:   color: var(--muted);
279:   font-size: 1.1rem;
280: }
281: 
282: .section-heading {
283:   margin-bottom: 1.5rem;
284: }
285: 
286: .section-heading h2 {
287:   margin-top: 0;
288: }
289: 
290: .section-heading p:last-child {
291:   color: var(--muted);
292: }
293: 
294: .category-grid {
295:   display: grid;
296:   gap: 1rem;
297: }
298: 
299: .category-card {
300:   background: rgba(17, 24, 39, 0.78);
301:   border: 1px solid var(--border);
302:   border-radius: var(--radius);
303:   padding: 1.25rem;
304:   transition: border-color 160ms ease, box-shadow 160ms ease, transform 160ms ease;
305: }
306: 
307: .category-card:hover {
308:   border-color: var(--accent);
309:   box-shadow: 0 18px 45px rgba(0, 0, 0, 0.18);
310: }
311: 
312: .category-card[open] {
313:   border-color: var(--accent);
314: }
315: 
316: .category-card summary {
317:   cursor: pointer;
318:   list-style: none;
319: }
320: 
321: .category-card summary::-webkit-details-marker {
322:   display: none;
323: }
324: 
325: .category-card summary span {
326:   display: flex;
327:   align-items: baseline;
328:   justify-content: space-between;
329:   gap: 1rem;
330: }
331: 
332: .category-card summary strong {
333:   color: var(--text);
334:   font-size: 1.15rem;
335: }
336: 
337: .category-card summary small {
338:   color: var(--accent);
339:   font-weight: 700;
340: }
341: 
342: .category-card > p {
343:   color: var(--muted);
344:   margin: 1rem 0 1.25rem;
345: }
346: 
347: .category-project-list {
348:   display: grid;
349:   gap: 1rem;
350: }
351: 
352: .project-list-card {
353:   background: rgba(15, 23, 42, 0.72);
354:   border: 1px solid var(--border);
355:   border-radius: calc(var(--radius) - 4px);
356:   padding: 1rem;
357: }
358: 
359: .project-list-card h3 {
360:   margin: 0 0 0.4rem;
361:   font-size: 1.05rem;
362: }
363: 
364: .project-list-card p {
365:   color: var(--muted);
366:   margin: 0;
367: }
368: 
369: .hero-card {
370:   display: grid;
371:   grid-template-columns: minmax(0, 1.4fr) minmax(220px, 0.6fr);
372:   align-items: center;
373:   gap: 2.5rem;
374: }
375: 
376: .hero-content {
377:   min-width: 0;
378: }
379: 
380: .hero-summary {
381:   max-width: 680px;
382:   color: var(--text);
383:   font-size: 1.15rem;
384: }
385: 
386: .hero-photo-wrap {
387:   display: flex;
388:   justify-content: center;
389: }
390: 
391: .hero-photo {
392:   width: min(360px, 100%);
393:   aspect-ratio: 1;
394:   object-fit: cover;
395:   border-radius: 30px;
396:   border: 3px solid var(--accent);
397:   box-shadow: 0 24px 70px rgba(0, 0, 0, 0.35);
398: }
399: 
400: .astro-code {
401:   border: 1px solid var(--border);
402:   border-radius: var(--radius);
403:   padding: 1.25rem;
404:   overflow-x: auto;
405:   line-height: 1.6;
406:   font-size: 0.95rem;
407: }
408: 
409: .astro-code code {
410:   font-family: Consolas, Monaco, "Courier New", monospace;
411: }
412: 
413: @media (min-width: 860px) {
414:   .category-grid {
415:     grid-template-columns: repeat(2, minmax(0, 1fr));
416:   }
417: 
418:   .category-card {
419:     align-self: start;
420:   }
421: }
422: 
423: .fade-in {
424:   animation: fadeInLeft 900ms ease both;
425: }
426: 
427: .fade-in:nth-child(n + 2) {
428:   animation-delay: 200ms;
429: }
430: 
431: .hover-category-card {
432:   min-height: 8rem;
433:   overflow: hidden;
434:   transition:
435:     min-height 220ms ease,
436:     border-color 180ms ease,
437:     box-shadow 180ms ease;
438: }
439: 
440: .category-card-body {
441:   max-height: 0;
442:   opacity: 0;
443:   overflow: hidden;
444:   transform: translateY(-0.5rem);
445:   transition:
446:     max-height 250ms ease,
447:     opacity 200ms ease,
448:     transform 200ms ease;
449: }
450: 
451: .hover-category-card:hover .category-card-body,
452: .hover-category-card:focus-within .category-card-body {
453:   max-height: 900px;
454:   opacity: 1;
455:   transform: translateY(0);
456: }
457: 
458: .hover-category-card:hover,
459: .hover-category-card:focus-within {
460:   min-height: 27rem;
461:   border-color: var(--accent);
462: }
463: 
464: .hover-category-card:hover .category-card-body,
465: .hover-category-card:focus-within .category-card-body {
466:   max-height: 24rem;
467:   opacity: 1;
468:   transform: translateY(0);
469: }
470: 
471: .category-carousel {
472:   display: grid;
473:   gap: 0.85rem;
474:   margin-top: 1rem;
475: }
476: 
477: .carousel-controls {
478:   display: flex;
479:   align-items: center;
480:   justify-content: flex-end;
481:   gap: 0.65rem;
482: }
483: 
484: .carousel-button {
485:   width: 2rem;
486:   height: 2rem;
487:   border: 1px solid var(--border);
488:   border-radius: 999px;
489:   background: rgba(15, 23, 42, 0.75);
490:   color: var(--text);
491:   cursor: pointer;
492:   font-weight: 800;
493:   line-height: 1;
494: }
495: 
496: .carousel-button:hover,
497: .carousel-button:focus-visible {
498:   border-color: var(--accent);
499:   color: var(--accent);
500: }
501: 
502: .carousel-count {
503:   color: var(--muted);
504:   font-size: 0.85rem;
505:   font-weight: 700;
506: }
507: 
508: .category-project-window {
509:   min-height: 17rem;
510: }
511: 
512: .project-slide {
513:   display: none;
514: }
515: 
516: .project-slide.is-active {
517:   display: grid;
518:   gap: 0.85rem;
519: }
520: 
521: .project-slide-image,
522: .project-image-placeholder {
523:   width: 100%;
524:   height: 11rem;
525:   border: 1px solid var(--border);
526:   border-radius: var(--radius);
527:   background: rgba(15, 23, 42, 0.75);
528: }
529: 
530: .project-slide-image {
531:   object-fit: contain;
532:   background: #f8fafc;
533: }
534: 
535: .project-image-placeholder {
536:   display: grid;
537:   place-items: center;
538:   color: var(--muted);
539:   font-weight: 700;
540: }
541: 
542: .project-slide-content {
543:   display: grid;
544:   gap: 0.55rem;
545: }
546: 
547: .project-slide-content h3,
548: .project-slide-content p {
549:   margin: 0;
550: }
551: 
552: .project-slide-content h3 a {
553:   color: var(--text);
554:   text-decoration: none;
555:   transition: color 160ms ease;
556: }
557: 
558: .project-slide:hover .project-slide-content h3 a,
559: .project-slide-content h3 a:hover,
560: .project-slide-content h3 a:focus-visible {
561:   color: var(--accent);
562: }
563: 
564: .category-card-header {
565:   min-height: 3rem;
566: }
567: 
568: .category-card-header strong {
569:   transition: color 160ms ease;
570: }
571: 
572: .hover-category-card:hover .category-card-header strong,
573: .hover-category-card:focus-within .category-card-header strong {
574:   color: var(--accent);
575: }
576: 
577: .course-track-grid,
578: .syllabus-grid {
579:   display: grid;
580:   gap: 1rem;
581: }
582: 
583: .course-track-card,
584: .syllabus-card {
585:   background: rgba(17, 24, 39, 0.78);
586:   border: 1px solid var(--border);
587:   border-radius: var(--radius);
588:   padding: 1.25rem;
589:   transition: transform 160ms ease, border-color 160ms ease, box-shadow 160ms ease;
590: }
591: 
592: .course-track-card:hover,
593: .syllabus-card:hover {
594:   transform: translateY(-3px);
595:   border-color: var(--accent);
596:   box-shadow: 0 18px 45px rgba(0, 0, 0, 0.18);
597: }
598: 
599: .course-track-card h3,
600: .syllabus-card h3 {
601:   margin-top: 0;
602:   margin-bottom: 0.5rem;
603: }
604: 
605: .course-track-card p,
606: .syllabus-card p {
607:   color: var(--muted);
608: }
609: 
610: .course-area {
611:   color: var(--accent);
612:   font-size: 0.78rem;
613:   font-weight: 800;
614:   letter-spacing: 0.12em;
615:   text-transform: uppercase;
616:   margin: 0 0 0.4rem;
617: }
618: 
619: .syllabus-card {
620:   display: flex;
621:   flex-direction: column;
622:   justify-content: space-between;
623:   gap: 1rem;
624: }
625: 
626: .text-link {
627:   color: var(--link);
628:   font-weight: 800;
629: }
630: 
631: .text-link:hover {
632:   color: var(--accent);
633: }
634: 
635: .coursework-callout {
636:   display: grid;
637:   gap: 1.5rem;
638:   align-items: center;
639: }
640: 
641: .coursework-callout h2 {
642:   margin-top: 0;
643:   margin-bottom: 0.75rem;
644: }
645: 
646: .coursework-callout p {
647:   color: var(--muted);
648:   max-width: 78ch;
649: }
650: 
651: .coursework-callout-action {
652:   display: flex;
653:   justify-content: flex-start;
654: }
655: 
656: .contact-details {
657:   display: grid;
658:   gap: 1rem;
659:   margin-top: 1.5rem;
660: }
661: 
662: .contact-details div {
663:   background: rgba(15, 23, 42, 0.65);
664:   border: 1px solid var(--border);
665:   border-radius: var(--radius);
666:   padding: 1rem;
667: }
668: 
669: .contact-details span {
670:   display: block;
671:   color: var(--accent);
672:   font-size: 0.78rem;
673:   font-weight: 800;
674:   letter-spacing: 0.12em;
675:   text-transform: uppercase;
676:   margin-bottom: 0.35rem;
677: }
678: 
679: .contact-details p,
680: .contact-details a {
681:   margin: 0;
682:   color: var(--text);
683:   font-weight: 700;
684:   overflow-wrap: anywhere;
685: }
686: 
687: .contact-details a:hover {
688:   color: var(--accent);
689: }
690: 
691: @media (min-width: 760px) {
692:   .contact-details {
693:     grid-template-columns: repeat(2, minmax(0, 1fr));
694:   }
695: }
696: 
697: @media (min-width: 820px) {
698:   .coursework-callout {
699:     grid-template-columns: minmax(0, 1fr) auto;
700:   }
701: 
702:   .coursework-callout-action {
703:     justify-content: flex-end;
704:   }
705: }
706: 
707: @media (min-width: 760px) {
708:   .course-track-grid {
709:     grid-template-columns: repeat(2, minmax(0, 1fr));
710:   }
711: 
712:   .syllabus-grid {
713:     grid-template-columns: repeat(3, minmax(0, 1fr));
714:   }
715: }
716: 
717: @keyframes fadeInLeft {
718:   from {
719:     opacity: 0;
720:     transform: translateX(-12px);
721:   }
722: 
723:   to {
724:     opacity: 1;
725:     transform: translateX(0);
726:   }
727: }
728: 
729: @media (min-width: 900px) {
730:   .project-slide.is-active {
731:     grid-template-columns: 14rem 1fr;
732:     align-items: start;
733:   }
734: 
735:   .project-slide-image,
736:   .project-image-placeholder {
737:     height: 9rem;
738:   }
739: }
740: 
741: @media (max-width: 760px) {
742:   .nav-container {
743:     align-items: flex-start;
744:     flex-direction: column;
745:     gap: 1rem;
746:   }
747: 
748:   .nav-links {
749:     flex-wrap: wrap;
750:     gap: 0.85rem;
751:   }
752: 
753:   .site-main {
754:     padding: 2rem 1rem;
755:   }
756: 
757:   .section-action {
758:     margin: 10px;
759:   }
760: 
761:   .section-card {
762:     padding: 1.35rem;
763:   }
764: 
765:   .project-grid {
766:     grid-template-columns: 1fr;
767:   }
768: 
769:   .hero-card {
770:     grid-template-columns: 1fr;
771:     text-align: left;
772:   }
773: 
774:   .hero-photo-wrap {
775:     justify-content: flex-start;
776:     order: -1;
777:   }
778: 
779:   .hero-photo {
780:     width: 240px;
781:   }
782: }
````

## File: tsconfig.json
````json
1: {
2:   "extends": "astro/tsconfigs/strict",
3:   "include": [".astro/types.d.ts", "**/*"],
4:   "exclude": ["dist"]
5: }
````

## File: src/pages/index.astro
````astro
  1: ---
  2: import BaseLayout from "../layouts/BaseLayout.astro";
  3: 
  4: const featuredProjects = [
  5:   {
  6:     title: "SportsPro Technical Support",
  7:     href: "/projects/sportspro/",
  8:     summary:
  9:       "ASP.NET Core MVC support management system with database-backed CRUD workflows.",
 10:     tech: ["C#", "ASP.NET Core", "Entity Framework", "SQL Server"],
 11:   },
 12:   {
 13:     title: "Godot Grid Roguelike",
 14:     href: "/projects/godot-roguelike/",
 15:     summary:
 16:       "Turn-based roguelike prototype with grid movement, combat, rewards, and persistent run state.",
 17:     tech: ["Godot", "C#", "Game Systems"],
 18:   },
 19:   {
 20:     title: "Display Switching CLI",
 21:     href: "/projects/display-switcher/",
 22:     summary:
 23:       "Go command-line tool for switching Windows display profiles and launching workflow-specific apps.",
 24:     tech: ["Go", "Cobra", "JSON"],
 25:   },
 26: ];
 27: 
 28: const skillGroups = [
 29:   {
 30:     name: "Languages",
 31:     skills: ["C#", "PHP", "JavaScript", "Go", "SQL", "HTML/CSS"],
 32:   },
 33:   {
 34:     name: "Frameworks & Tools",
 35:     skills: ["ASP.NET Core MVC", "Entity Framework", "Godot", "Cobra", "Laravel", "React", "WAMP/LAMP"],
 36:   },
 37:   {
 38:     name: "Databases & Concepts",
 39:     skills: ["MySQL", "SQL Server", "SQLite", "REST APIs", "CRUD", "MVC"],
 40:   },
 41: ];
 42: 
 43: const contactDetails = {
 44:   email: "jared.cstreet@gmail.com",
 45:   phone: "605-999-0122",
 46:   location: "Sioux Falls, SD",
 47:   github: "https://github.com/OhStreet",
 48:   linkedin: "www.linkedin.com/in/jared-street-a63008400",
 49:   resume: "/documents/JaredStreetResume.pdf",
 50: };
 51: ---
 52: 
 53: <BaseLayout
 54:   title="Jared Street | Entry-Level Software Developer"
 55:   description="Portfolio for Jared Street, an entry-level software developer focused on practical web, database, and application projects."
 56: >
 57:   <section id="hero" class="section-card hero-card">
 58:     <div class="hero-content fade-in">
 59:       <p class="eyebrow">Entry-Level Software Developer</p>
 60: 
 61:       <h1>Jared Street</h1>
 62: 
 63:       <p class="hero-summary">
 64:         I build practical web, database, and application projects using C#,
 65:         ASP.NET Core, PHP, SQL, JavaScript, and Go.
 66:       </p>
 67: 
 68:       <div class="button-row">
 69:         <a class="button button-primary" href="/projects/">View Projects</a>
 70:         <a class="button button-primary" href="/documents/JaredStreetResume.pdf">View Resume</a>
 71:       </div>
 72:     </div>
 73: 
 74:     <div class="hero-photo-wrap fade-in">
 75:       <img
 76:         class="hero-photo"
 77:         src="/screenshots/tempheadshot.jpeg"
 78:         alt="Headshot of Jared Street"
 79:       />
 80:     </div>
 81:    
 82:   </section>
 83: 
 84:   <section id="featured-projects" class="fade-in">
 85:     <div class="section-heading">
 86:       <p class="eyebrow">Selected Work</p>
 87:       <h2>Featured Projects</h2>
 88:       <p>
 89:         A few projects that best represent my experience with web applications,
 90:         database-backed systems, tools, and C# development.
 91:       </p>
 92:     </div>
 93: 
 94:     <div class="project-grid ">
 95:       {featuredProjects.map((project) => (
 96:         <article class="project-card">
 97:           <h3>
 98:             <a href={project.href}>{project.title}</a>
 99:           </h3>
100: 
101:           <p>{project.summary}</p>
102: 
103:           <div class="tech-list">
104:             {project.tech.map((techItem) => (
105:               <span class="tech-pill">{techItem}</span>
106:             ))}
107:           </div>
108: 
109:           <div class="button-row">
110:             <a class="button button-secondary" href={project.href}>
111:               View Project
112:             </a>
113:           </div>
114:         </article>
115:       ))}
116:     </div>
117: 
118:     <div class="section-action">
119:       <a class="button button-primary" href="/projects/">View All Projects</a>
120:     </div>
121:   </section>
122: 
123:   <section id="skills" class="fade-in">
124:     <div class="section-heading fade-in">
125:       <p class="eyebrow">Technical Stack</p>
126:       <h2>Skills</h2>
127:       <p>
128:         Technologies and concepts I have used across coursework, portfolio projects,
129:         and independent development.
130:       </p>
131:     </div>
132: 
133:     <div class="skills-grid fade-in">
134:       {skillGroups.map((group) => (
135:         <article class="skill-card">
136:           <h3>{group.name}</h3>
137: 
138:           <div class="tech-list">
139:             {group.skills.map((skill) => (
140:               <span class="tech-pill">{skill}</span>
141:             ))}
142:           </div>
143:         </article>
144:       ))}
145:     </div>
146:   </section>
147: 
148:   <section id="contact" class="section-card contact-card fade-in">
149:     <p class="eyebrow">Contact</p>
150:     <h2>Let’s Connect</h2>
151: 
152:     <p>
153:       I am preparing to apply for entry-level software development roles and am
154:       interested in practical application development, web systems, database-backed
155:       projects, and developer tools.
156:     </p>
157: 
158:     <div class="contact-details">
159:       <div>
160:         <span>Email</span>
161:         <a href={`mailto:${contactDetails.email}`}>{contactDetails.email}</a>
162:       </div>
163: 
164:       <div>
165:         <span>Phone</span>
166:         <a href={`tel:${contactDetails.phone}`}>{contactDetails.phone}</a>
167:       </div>
168: 
169:       <div>
170:         <span>Location</span>
171:         <p>{contactDetails.location}</p>
172:       </div>
173:     </div>
174: 
175:     <div class="button-row">
176:       <a class="button button-primary" href={contactDetails.resume}>
177:         View Resume
178:       </a>
179: 
180:       <a
181:         class="button button-secondary"
182:         href={contactDetails.github}
183:         target="_blank"
184:         rel="noopener noreferrer"
185:       >
186:         GitHub
187:       </a>
188: 
189:       <a
190:         class="button button-secondary"
191:         href={contactDetails.linkedin}
192:         target="_blank"
193:         rel="noopener noreferrer"
194:       >
195:         LinkedIn
196:       </a>
197:     </div>
198:   </section>
199: </BaseLayout>
````
