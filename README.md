# Bluecress 1.0 TEST
Native Android Cube color-exchange puzzle. Android 8+ (min26), target35. Package com.gg007.bluecress. Twelve original mixed-color starts on a compact 3x2 board.

## Rules
Cube color-exchange puzzle on a compact 3-column by 2-row board. Press NORTH, EAST, SOUTH or WEST to roll the cube one cell in that direction. After rotating, its new DOWN face and the landing tile swap blue/plain colors. A plain face on blue picks it up; a blue face on plain drops it; matching colors stay unchanged. There are always six blue marks across board and cube combined. Goal: all six cube faces blue and all board tiles plain, at any position. CHECK confirms. Gold ring marks the cube position without hiding the tile underneath. The unfolded cube shows all six CURRENT WORLD faces: UP, DOWN, NORTH, SOUTH, EAST, WEST. Labels stay world-relative as the cube colors rotate. Twelve original mixed-color starts with shortest solutions of 4-9 rolls. This is a smaller training adaptation of standard Cube, with blue already on some faces at the start and an unfolded display instead of 3D. No initial exchange occurs until a roll. Rolling back is not an undo; use UNDO to restore both color states. Unlimited undo/reset, next and level selection. Saved palette and optional a-f board tile guides.

## Download and status
https://mega.co.nz/#!wdNBDJ7A!PDVEJuwioVncTO3_CdjcClbzZIynM3RaGyYojHcteo8
APK SHA256 81bc181d4f3a227d5c5fe49c34c20e776b7fb48fdd21fcbdc49eb43a159c9baa; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
Reverse breadth-first search from all six goal positions reaches all 5,544 states with exactly six blue marks across six cube faces and six board tiles, maximum distance 17. Across all these states and four directions, 22,176 comparisons agree between production face-index rotation/XOR exchange and an independent physical normal-vector rotation plus boolean exchange oracle. Blue count stays six and off-board rolls are rejected. Twelve independent forward searches prove shortest solution lengths 4,4,5,5,6,6,7,7,8,8,9,9. Bounds, invalid state, early check, undo, solved lock, reset and route replay pass. Archived portable generator reproduces levels and the archived Java oracle reruns with byte-equal source. Actual drawing-adapter directional touch, solve/undo/replay, menu, levels, privacy and saved palette/tile guides pass. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 175 prior studio mechanics and all 803 web registry records. Cubeward rolls a fixed numbered cube to a dock with a target top face; neither its board nor its face labels exchange colors. Bluecress changes both board and face colors on every landing, aims for all six faces blue, and has no dock. This persistent board/cube color exchange, rather than orientation routing alone, is the distinct algorithm and planning problem. No Cube color-exchange functional match found in the reviewed catalog. Known Cube adaptation, not a global invention claim. Original generated starts, implementation and visuals; no source puzzle boards, code or art copied. Recovered repository corpus remains partial.
Rules https://www.chiark.greenend.org.uk/~sgtatham/puzzles/doc/cube.html ; independent rules https://www.mobygames.com/game/107459/cube/ .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/bluecress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.bluecress.BoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Bluecress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, tile guides and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 176-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/07s8ffjvp34v-bluecress-source-archive . Repository https://github.com/iLanis-agent/bluecress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
