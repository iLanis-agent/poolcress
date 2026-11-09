# Poolcress 1.0 TEST
Native Android Reflect Link room-length-set loop puzzle. Android 8+ (min26), target35. Package com.gg007.poolcress. Twelve original unique boards on a compact 5x4 grid.

## Rules
Rail Pool on a 5-column, 4-row grid. Draw one noncrossing closed loop through ALL twenty cell centers. Every cell has exactly two roads; no branches, separate cycles or unused cells. Each outlined room may list a pool of lengths: the SET of all different full straight-run lengths that visit any cell in that room, including a run ending at a turn there. Count EDGES between neighboring centers, not cells. Continue past room borders until a turn. Each listed length must appear and no other length may appear in that room; repeated runs of one allowed length are fine. Rooms marked any have no length restriction. Room borders do not limit visits. No question-mark clues in this edition. Tap gaps between centers to toggle roads. Undo/reset, levels and next; saved palette and optional room labels. No timer or score.

## Download and status
https://mega.co.nz/#!ZIE0TYhK!ojLkmeGZt-iBfem0VO9WDUaQ8Y1jz7nPjDkmfGvX5-Q
APK SHA256 b2938e35bd4ff92a2ead62527bc99f1b22bfd819c3796b60421645e097e7818a; 20974 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Production bit-direction tracing agrees with an independent coordinate adjacency and flood-fill oracle on all 54 spanning degree-two covers of the 5x4 grid: exactly 14 are single Hamilton loops. Every one of the 648 board/candidate checks agrees; all straight-run length sets on the 14 loops match an independent ordered-route grouping oracle. Another 200,000 deterministic random edge masks agree on topology. The portable seed-641109 generator enumerates all Hamilton routes, grows connected room layouts and removes whole room pools only while one solution remains. Twelve original room/clue boards each have exactly one solution and all twelve loops differ. Whole-run continuation across room borders, both run endpoints, repeated lengths as sets, bounds, toggle/clear, undo/reset, solved lock and malformed states pass. Actual drawing-adapter taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/room labels. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 195 prior live studio descriptions and byte-current 803 web registry entries using functional terms. No Rail Pool/whole-run length-set match in this partial corpus. Cloverroad counts visited cells per room and limits room entry; Bendhollow counts bends per room; Pipecress fixes pipe shapes and permits straight crossings; Runebriar constrains individual circle arms. Poolcress instead visits all twenty cells without crossing and matches per-room SETS of complete straight-run edge lengths, continuing across room borders and counting one run in every room its cells visit. Known Rail Pool adaptation with original generated boards, code and visuals; no copied layouts/code/art or global invention claim. Publisher rules, constructor rules and community descriptions agree on the core constraints. No history claim.
Rules https://brokensign.com/puzzle/2022/05/01/rail-pool.html ; independent rules https://www.gmpuzzles.com/blog/2022/12/rail-pool-by-martin-ender/ .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/poolcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.poolcress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Poolcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, room labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 196-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/pjygfbxb2mrp-poolcress-source-archive . Repository https://github.com/iLanis-agent/poolcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
