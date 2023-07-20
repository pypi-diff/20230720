# Comparing `tmp/music-assistant-frontend-2.0.4.tar.gz` & `tmp/music-assistant-frontend-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-assistant-frontend-2.0.4.tar", last modified: Thu Jul 20 16:34:21 2023, max compression
+gzip compressed data, was "music-assistant-frontend-2.0.5.tar", last modified: Thu Jul 20 17:58:26 2023, max compression
```

## Comparing `music-assistant-frontend-2.0.4.tar` & `music-assistant-frontend-2.0.5.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.823826 music-assistant-frontend-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 16:32:47.000000 music-assistant-frontend-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 16:32:47.000000 music-assistant-frontend-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 16:34:21.823826 music-assistant-frontend-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-20 16:32:47.000000 music-assistant-frontend-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.795827 music-assistant-frontend-2.0.4/music_assistant_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.823826 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AddProvider-a95ca786.js
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AlbumDetails-55ac33a4.js
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-4d78da02.js
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-c80b13d7.css
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ArtistDetails-7c7516d2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/BrowseView-457188ac.js
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Button-15e2fa72.css
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Button-4a781169.js
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-282a676b.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-ed1c67df.css
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/CoreConfigs-1c0e2549.css
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/CoreConfigs-69940384.js
--rw-r--r--   0 runner    (1001) docker     (123)    56884 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-4e51f0b8.js
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-8766b49d.css
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig-25e44c20.css
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditCoreConfig-714d074a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditPlayer-f0c55a15.js
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditProvider-a2553a06.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/HomeView-af5707e7.js
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/HomeView-f559b858.css
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader-32cd2df9.css
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing-7290acd0.css
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryAlbums-757b8aa2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryArtists-225ce0c1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryPlaylists-4ffdc19f.js
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryRadios-a948d358.js
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryTracks-5a540fa3.js
--rw-r--r--   0 runner    (1001) docker     (123)    33420 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-2bd74fad.js
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-732a7603.css
--rw-r--r--   0 runner    (1001) docker     (123)   160576 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
--rw-r--r--   0 runner    (1001) docker     (123)   347588 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   125116 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   143452 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PanelviewItem-14a6b77a.css
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlayerQueue-7ca94b07.js
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Players-5c99fe5e.js
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlaylistDetails-f8a1c191.js
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Providers-0e527c0c.css
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Providers-65d3d824.js
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/RadioDetails-71dc877e.js
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Search-f31ee239.js
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Settings-f159e60c.js
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/TrackDetails-ca02e9b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-12aff0c7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-9c063078.css
--rw-r--r--   0 runner    (1001) docker     (123)    26417 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-61e39030.js
--rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-76f512af.css
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-103d8462.css
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-f3e11b51.js
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-28e4e64e.css
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-93a2100b.js
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-adefbf87.js
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-bc1524a3.css
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-75456689.js
--rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VGrid-b9c72806.css
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-b9e24cb0.css
--rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-f848c028.js
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-b930657a.css
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-ccc026f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VRow-74a0e5a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-45a454b3.css
--rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-a66ffc02.js
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSpacer-159b0383.js
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-21d8affa.js
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-3cd3e980.css
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-222d6375.css
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-806969a3.js
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_dark-75402cd0.png
--rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_light-b832ae9e.png
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/crossfade-ba51f69a.png
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/hires-438c7046.png
--rw-r--r--   0 runner    (1001) docker     (123)   402667 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ade73b84.js
--rw-r--r--   0 runner    (1001) docker     (123)   662925 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ecb9e627.css
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index.browser-7e542916.js
--rw-r--r--   0 runner    (1001) docker     (123)    28226 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/layout-b0232ef9.js
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/logo-c9d5d6ab.png
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/m4a-45331b05.png
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1280212 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot
--rw-r--r--   0 runner    (1001) docker     (123)   576748 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff
--rw-r--r--   0 runner    (1001) docker     (123)  1279992 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   396732 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-20 16:34:09.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-20 16:34:09.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/workbox-27b29e6f.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.795827 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:34:19.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 16:33:17.000000 music-assistant-frontend-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:34:21.827826 music-assistant-frontend-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:58:26.361452 music-assistant-frontend-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 17:57:15.000000 music-assistant-frontend-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 17:57:15.000000 music-assistant-frontend-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 17:58:26.361452 music-assistant-frontend-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-20 17:57:15.000000 music-assistant-frontend-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:58:26.341452 music-assistant-frontend-2.0.5/music_assistant_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:58:26.361452 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/AddProvider-fa211913.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/AlbumDetails-ef8a3bee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Alert-a5ce795e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Alert-c80b13d7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ArtistDetails-cd5389ba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/BrowseView-d5fa89c1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Button-00834c6c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Button-15e2fa72.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Container-4773c160.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Container-ed1c67df.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/CoreConfigs-1c0e2549.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/CoreConfigs-ec75d11a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56884 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Default-7879cbcb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Default-8766b49d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditConfig-25e44c20.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditCoreConfig-37eaad58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditPlayer-33767eb3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditProvider-f88730fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/HomeView-95da878e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/HomeView-f559b858.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/InfoHeader-32cd2df9.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ItemsListing-7290acd0.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryAlbums-55bc0ec5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryArtists-0afc0ed9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryPlaylists-86c14bd9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryRadios-3bd5ccff.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryTracks-07ab288b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ListviewItem-707ff3c9.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33420 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ListviewItem-e2342ce8.js
+-rw-r--r--   0 runner    (1001) docker     (123)   160576 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   347588 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   125116 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   143452 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PanelviewItem-14a6b77a.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PlayerQueue-6206a6c6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Players-73f88aa0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PlaylistDetails-ad67ce68.js
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Providers-0e527c0c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Providers-0fb3a52e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/RadioDetails-fb9a6d90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Search-1975e9f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Settings-05fc67af.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/TrackDetails-3d9e1c6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBadge-9c063078.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBadge-f7d58168.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26417 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBtn-629f5316.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBtn-76f512af.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VCard-04ae357c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VCard-103d8462.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDialog-28e4e64e.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDialog-667c0916.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDivider-bc1524a3.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDivider-df9414f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VExpansionPanel-1ca09b07.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VGrid-b9c72806.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VListItem-39677d21.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VListItem-b9e24cb0.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VMenu-240a4406.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VMenu-b930657a.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VRow-7d86481a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VSelect-45a454b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VSelect-4d69c543.js
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VSpacer-82874439.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VTabs-3cd3e980.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VTabs-f388999c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VToolbar-222d6375.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VToolbar-b79315e8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/cover_dark-75402cd0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/cover_light-b832ae9e.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/crossfade-ba51f69a.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/hires-438c7046.png
+-rw-r--r--   0 runner    (1001) docker     (123)   402427 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/index-a5bb9833.js
+-rw-r--r--   0 runner    (1001) docker     (123)   662925 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/index-ecb9e627.css
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/index.browser-7e542916.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28226 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/layout-ff13c6fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/logo-c9d5d6ab.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/m4a-45331b05.png
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1280212 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   576748 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  1279992 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   396732 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 17:58:14.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/pwa-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/pwa-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 17:58:11.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-20 17:58:16.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-20 17:58:16.000000 music-assistant-frontend-2.0.5/music_assistant_frontend/workbox-27b29e6f.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:58:26.341452 music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 17:58:25.000000 music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-20 17:58:26.000000 music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:58:25.000000 music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:58:24.000000 music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 17:58:26.000000 music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 17:57:39.000000 music-assistant-frontend-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:58:26.361452 music-assistant-frontend-2.0.5/setup.cfg
```

### Comparing `music-assistant-frontend-2.0.4/LICENSE` & `music-assistant-frontend-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/PKG-INFO` & `music-assistant-frontend-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.0.4
+Version: 2.0.5
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.0.4/README.md` & `music-assistant-frontend-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/apple-touch-icon.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AddProvider-a95ca786.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/AddProvider-fa211913.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -16,37 +16,37 @@
     x as l,
     A as a,
     K as c,
     N as d,
     v as y,
     L as r,
     M as v
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as P
-} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js";
 import {
     b as T,
     V as _,
     c as $
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as A
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     j as I
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     c as O
-} from "./VMenu-ccc026f2.js";
-import "./VExpansionPanel-75456689.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSpacer-159b0383.js";
-import "./VSelect-a66ffc02.js";
+} from "./VMenu-240a4406.js";
+import "./VExpansionPanel-1ca09b07.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSpacer-82874439.js";
+import "./VSelect-4d69c543.js";
 const U = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AlbumDetails-55ac33a4.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/AlbumDetails-ef8a3bee.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -9,63 +9,62 @@
     q as p,
     y as k,
     j as i,
     x as s,
     v as b,
     F,
     z as P,
-    M as h,
+    M as y,
     L as C,
     ai as R,
-    K as y,
+    K as h,
     N as c,
     A as S,
     ah as j
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as V,
     f as w
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
 import {
     _ as q
-} from "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js";
+} from "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js";
 import {
     C as I,
     L as H,
     a as K
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as O
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as U
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as G
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     a as J
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     l as Q
-} from "./VBtn-61e39030.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js"; /* empty css              */
-import "./layout-b0232ef9.js";
+} from "./VBtn-629f5316.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js"; /* empty css              */
+import "./layout-ff13c6fd.js";
 const W = C("br", null, null, -1),
     X = C("br", null, null, -1),
-    ke = L({
+    _e = L({
         __name: "AlbumDetails",
         props: {
             itemId: {},
             provider: {},
             forceProviderVersion: {}
         },
         setup(A) {
@@ -148,44 +147,45 @@
                             height: "55px"
                         }
                     }, null, 8, ["title"]), i(U), i(I, null, {
                         default: s(() => [i(G, null, {
                             default: s(() => {
                                 var r;
                                 return [(p(!0), k(F, null, P((r = n.value) == null ? void 0 : r.provider_mappings, t => (p(), b(H, {
+                                    key: t.provider_instance,
                                     onClick: u => e.$router.push({
                                         name: "album",
                                         params: {
                                             itemId: t.item_id,
                                             provider: t.provider_instance
                                         }
                                     })
                                 }, {
                                     prepend: s(() => [i(K, {
                                         domain: t.provider_domain,
                                         size: 30
                                     }, null, 8, ["domain"])]),
-                                    title: s(() => [y(c(S(l).providerManifests[t.provider_domain].name), 1)]),
-                                    subtitle: s(() => [y(c(t.item_id) + " | " + c(t.audio_format.content_type) + " | " + c(t.audio_format.sample_rate / 1e3) + "kHz/" + c(t.audio_format.bit_depth) + " bits ", 1)]),
+                                    title: s(() => [h(c(S(l).providerManifests[t.provider_domain].name), 1)]),
+                                    subtitle: s(() => [h(c(t.item_id) + " | " + c(t.audio_format.content_type) + " | " + c(t.audio_format.sample_rate / 1e3) + "kHz/" + c(t.audio_format.bit_depth) + " bits ", 1)]),
                                     append: s(() => [t.url ? (p(), b(Q, {
                                         key: 0,
                                         variant: "plain",
                                         icon: "mdi-open-in-new",
                                         onClick: j(u => T(t.url), ["prevent"])
-                                    }, null, 8, ["onClick"])) : h("", !0)]),
+                                    }, null, 8, ["onClick"])) : y("", !0)]),
                                     _: 2
-                                }, 1032, ["onClick"]))), 256))]
+                                }, 1032, ["onClick"]))), 128))]
                             }),
                             _: 1
                         })]),
                         _: 1
                     })]),
                     _: 1
-                })) : h("", !0)]),
+                })) : y("", !0)]),
                 _: 1
             })]))
         }
     });
 export {
-    ke as
+    _e as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-4d78da02.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Alert-a5ce795e.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -12,21 +12,21 @@
     k,
     q as j,
     v as q,
     V as O,
     z as G,
     x as H,
     Y as M
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as N
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     e as Y
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     a as J,
     E as K,
     G as Q,
     b as U,
     o as W,
     p as X,
@@ -41,15 +41,15 @@
     s as re,
     g as ie,
     y as ce,
     w as ue,
     V as de,
     x as f,
     l as ve
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 const me = Y("v-alert-title"),
     ye = ["success", "info", "warning", "error"],
     fe = D({
         border: {
             type: [Boolean, String],
             validator: e => typeof e == "boolean" || ["top", "end", "bottom", "start"].includes(e)
         },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-c80b13d7.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Alert-c80b13d7.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ArtistDetails-7c7516d2.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ArtistDetails-cd5389ba.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -7,64 +7,63 @@
     af as N,
     b as S,
     q as d,
     y as k,
     j as i,
     x as s,
     v as b,
-    F as g,
-    z,
+    F as z,
+    z as F,
     M as _,
     L as A,
     K as y,
     N as h,
-    A as F,
-    ah as R
-} from "./index-ade73b84.js";
+    A as R,
+    ah as g
+} from "./index-a5bb9833.js";
 import {
     _ as w,
     f as I
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
 import {
     _ as j
-} from "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js";
+} from "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js";
 import {
     C,
     L as q,
     a as K
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as O
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as U
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as G
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     a as H
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     l as J
-} from "./VBtn-61e39030.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js"; /* empty css              */
-import "./layout-b0232ef9.js";
-const M = A("br", null, null, -1),
-    P = A("br", null, null, -1),
-    be = E({
+} from "./VBtn-629f5316.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js"; /* empty css              */
+import "./layout-ff13c6fd.js";
+const P = A("br", null, null, -1),
+    Q = A("br", null, null, -1),
+    ve = E({
         __name: "ArtistDetails",
         props: {
             itemId: {},
             provider: {}
         },
         setup(V) {
             const o = V,
@@ -110,28 +109,28 @@
                     "sort-keys": ["timestamp_added DESC", "sort_name", "sort_album"],
                     "update-available": n.value,
                     onRefreshClicked: a[0] || (a[0] = r => {
                         c(), n.value = !1
                     }),
                     title: e.$t("tracks"),
                     checksum: e.provider + e.itemId
-                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), M, i(w, {
+                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), P, i(w, {
                     itemtype: "artistalbums",
                     "parent-item": l.value,
                     "show-provider": !1,
                     "show-favorites-only-filter": !1,
                     "load-data": D,
                     "sort-keys": ["timestamp_added DESC", "sort_name", "year"],
                     "update-available": n.value,
                     onRefreshClicked: a[1] || (a[1] = r => {
                         c(), n.value = !1
                     }),
                     title: e.$t("albums"),
                     checksum: e.provider + e.itemId
-                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), P, e.provider == "library" ? (d(), b(H, {
+                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), Q, e.provider == "library" ? (d(), b(H, {
                     key: 0,
                     style: {
                         "margin-bottom": "10px"
                     }
                 }, {
                     default: s(() => [i(O, {
                         color: "transparent",
@@ -139,45 +138,46 @@
                         style: {
                             height: "55px"
                         }
                     }, null, 8, ["title"]), i(U), i(C, null, {
                         default: s(() => [i(G, null, {
                             default: s(() => {
                                 var r;
-                                return [(d(!0), k(g, null, z((r = l.value) == null ? void 0 : r.provider_mappings, t => (d(), b(q, {
+                                return [(d(!0), k(z, null, F((r = l.value) == null ? void 0 : r.provider_mappings, t => (d(), b(q, {
+                                    key: t.provider_instance,
                                     onClick: m => e.$router.push({
-                                        name: "album",
+                                        name: "artist",
                                         params: {
                                             itemId: t.item_id,
                                             provider: t.provider_instance
                                         }
                                     })
                                 }, {
                                     prepend: s(() => [i(K, {
                                         domain: t.provider_domain,
                                         size: 30
                                     }, null, 8, ["domain"])]),
-                                    title: s(() => [y(h(F(u).providerManifests[t.provider_domain].name), 1)]),
+                                    title: s(() => [y(h(R(u).providerManifests[t.provider_domain].name), 1)]),
                                     subtitle: s(() => [y(h(t.item_id), 1)]),
                                     append: s(() => [t.url ? (d(), b(J, {
                                         key: 0,
                                         variant: "plain",
                                         icon: "mdi-open-in-new",
-                                        onClick: R(m => $(t.url), ["prevent"])
+                                        onClick: g(m => $(t.url), ["prevent"])
                                     }, null, 8, ["onClick"])) : _("", !0)]),
                                     _: 2
-                                }, 1032, ["onClick"]))), 256))]
+                                }, 1032, ["onClick"]))), 128))]
                             }),
                             _: 1
                         })]),
                         _: 1
                     })]),
                     _: 1
                 })) : _("", !0)]),
                 _: 1
             })]))
         }
     });
 export {
-    be as
+    ve as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/BrowseView-457188ac.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/BrowseView-d5fa89c1.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -13,34 +13,34 @@
     v as m,
     M as c,
     A as V,
     O as L,
     B as f,
     ae as q,
     S as M
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     L as N,
     s as O
-} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
+} from "./ListviewItem-e2342ce8.js"; /* empty css                             */
 import {
     C as P
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     l as T,
     k as D
-} from "./VBtn-61e39030.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VListItem-f848c028.js";
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css              */
+} from "./VBtn-629f5316.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VListItem-39677d21.js";
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css              */
 const U = _({
     __name: "BrowseView",
     props: {
         path: {}
     },
     setup(d) {
         const t = d,
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Button-4a781169.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Button-00834c6c.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -3,21 +3,21 @@
     q as p,
     v as l,
     V as c,
     z as i,
     x as u,
     Y as _,
     k as f
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as v
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     l as d
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 const m = {
     props: {
         variant: {
             type: String,
             default: ""
         }
     },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-282a676b.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Container-4773c160.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -15,30 +15,30 @@
     l as L,
     A as o,
     X as f,
     O as r,
     p as P,
     g as b,
     u as B
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     b as T,
     V as w
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     l as A,
     V as _,
     a as H,
     d as D,
     i as F
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     a as S,
     V as N
-} from "./VListItem-f848c028.js"; /* empty css              */
+} from "./VListItem-39677d21.js"; /* empty css              */
 const h = (t, a) => {
         const e = t.__vccOpts || t;
         for (const [n, m] of a) e[n] = m;
         return e
     },
     O = {
         props: {
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-ed1c67df.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Container-ed1c67df.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/CoreConfigs-1c0e2549.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/CoreConfigs-1c0e2549.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/CoreConfigs-69940384.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/CoreConfigs-ec75d11a.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -20,39 +20,39 @@
     A as d,
     y as L,
     M as w,
     z as K,
     F as O,
     Q,
     K as U
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     C as k,
     L as G,
     a as J
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as T
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as B
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     a as W,
     E as X,
     d as Y,
     F as Z,
     i as ee,
     V as I
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     a as M
-} from "./VCard-f3e11b51.js";
-import "./VMenu-ccc026f2.js";
-import "./VListItem-f848c028.js"; /* empty css              */
+} from "./VCard-04ae357c.js";
+import "./VMenu-240a4406.js";
+import "./VListItem-39677d21.js"; /* empty css              */
 const te = x({
         fixedHeader: Boolean,
         fixedFooter: Boolean,
         height: [Number, String],
         hover: Boolean,
         ...W(),
         ...X(),
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-4e51f0b8.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Default-7879cbcb.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -63,22 +63,22 @@
     a7 as Dt,
     a8 as Ht,
     a9 as Wt,
     aa as Fe,
     ab as At,
     ac as Ft,
     ad as Ot
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     u as Be,
     a as Ut,
     V as ce,
     b as fe,
     c as Qt
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     m as tt,
     a as _e,
     b as lt,
     c as at,
     d as Re,
     u as ot,
@@ -89,72 +89,72 @@
     i as se,
     t as jt,
     V as D,
     j as nt,
     k as Gt,
     l as rt,
     n as Xt
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     m as Me,
     u as Ee,
     a as Kt,
     b as Zt,
     c as Jt
-} from "./layout-b0232ef9.js";
+} from "./layout-ff13c6fd.js";
 import {
     V as el,
     a as tl,
     b as ut
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     B as F
-} from "./Button-4a781169.js";
+} from "./Button-00834c6c.js";
 import {
     L as Z,
     _ as ve,
     C as ll
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as al,
     _ as ct,
     a as ol,
     i as il,
     b as sl,
     c as nl,
     g as Oe
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
 import {
     m as rl,
     V as $e,
     a as ul,
     b as cl
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as dt,
     a as dl,
     b as vl,
     c as ml,
     d as pl
-} from "./VExpansionPanel-75456689.js";
+} from "./VExpansionPanel-1ca09b07.js";
 import {
     V as ye
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as fl,
     a as vt,
     b as yl
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as hl
-} from "./VBadge-12aff0c7.js";
+} from "./VBadge-f7d58168.js";
 import {
     V as _l,
     a as gl
-} from "./VDialog-93a2100b.js"; /* empty css              */
+} from "./VDialog-667c0916.js"; /* empty css              */
 function bl(a) {
     let {
         rootEl: t,
         isSticky: o,
         layoutItemStyles: s
     } = a;
     const l = A(!1),
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-8766b49d.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Default-8766b49d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig-25e44c20.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditConfig-25e44c20.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -20,59 +20,59 @@
     K as w,
     N as h,
     M as F,
     A as p,
     L as V,
     aO as v,
     aP as H
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     a as ne,
     b as re,
     c as ve,
     d as me,
     V as pe
-} from "./VExpansionPanel-75456689.js";
+} from "./VExpansionPanel-1ca09b07.js";
 import {
     a as ce,
     i as le,
     I as be,
     L as Ve,
     j as ke,
     l as T
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     d as ge,
     e as he,
     m as fe,
     u as Ce,
     c as X,
     V as $e,
     f as Y
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 import {
     f as Ee
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     a as we,
     c as Se,
     d as Ue
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as qe
-} from "./VSpacer-159b0383.js";
+} from "./VSpacer-82874439.js";
 import {
     V as Ie
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     c as Pe,
     d as Z,
     V as D,
     b as Re
-} from "./VSelect-a66ffc02.js";
+} from "./VSelect-4d69c543.js";
 const Te = _({
         ...ce(),
         ...ge()
     }, "VForm"),
     Ae = ee()({
         name: "VForm",
         props: Te(),
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditCoreConfig-714d074a.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditCoreConfig-37eaad58.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -10,40 +10,40 @@
     K as m,
     N as u,
     A as d,
     v,
     L as i,
     M as f,
     O as n
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as $
-} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js";
 import {
     n as B
 } from "./index.browser-7e542916.js";
 import {
     b as O,
     V as p,
     c as E
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as h
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     j as S
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     c as T
-} from "./VMenu-ccc026f2.js";
-import "./VExpansionPanel-75456689.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSpacer-159b0383.js";
-import "./VSelect-a66ffc02.js";
+} from "./VMenu-240a4406.js";
+import "./VExpansionPanel-1ca09b07.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSpacer-82874439.js";
+import "./VSelect-4d69c543.js";
 const A = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditPlayer-f0c55a15.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditPlayer-33767eb3.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -10,36 +10,36 @@
     A as t,
     K as d,
     N as r,
     L as n,
     M as u,
     v as p,
     O as a
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     V as N,
     _ as B
-} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js";
 import {
     b as I,
     V as m,
     c as S
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as g
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as T
-} from "./VSelect-a66ffc02.js";
-import "./VExpansionPanel-75456689.js";
-import "./VBtn-61e39030.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VMenu-ccc026f2.js";
-import "./VSpacer-159b0383.js";
+} from "./VSelect-4d69c543.js";
+import "./VExpansionPanel-1ca09b07.js";
+import "./VBtn-629f5316.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VMenu-240a4406.js";
+import "./VSpacer-82874439.js";
 const P = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditProvider-a2553a06.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/EditProvider-f88730fc.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -13,43 +13,43 @@
     x as d,
     A as s,
     K as p,
     N as m,
     v as f,
     L as u,
     M as v
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     V as I,
     _ as O
-} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js";
 import {
     n as P
 } from "./index.browser-7e542916.js";
 import {
     b as U,
     V as _,
     c as x
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as h
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as A
-} from "./VSelect-a66ffc02.js";
+} from "./VSelect-4d69c543.js";
 import {
     j as D
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     c as q
-} from "./VMenu-ccc026f2.js";
-import "./VExpansionPanel-75456689.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSpacer-159b0383.js";
+} from "./VMenu-240a4406.js";
+import "./VExpansionPanel-1ca09b07.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSpacer-82874439.js";
 const z = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/HomeView-af5707e7.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/HomeView-95da878e.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 import {
     V as r,
     a as m
-} from "./VRow-74a0e5a5.js";
+} from "./VRow-7d86481a.js";
 import {
     a as c
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as p
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     l as d,
     V as u
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     l as _,
     r as f,
     q as i,
     y as o,
     L as l,
     j as a,
     x as t,
     F as h,
     z as b,
     v as g,
     N as V
-} from "./index-ade73b84.js"; /* empty css              */
+} from "./index-a5bb9833.js"; /* empty css              */
 const v = {
         style: {
             "margin-left": "10px",
             "margin-right": "10px",
             "margin-top": "10px",
             "margin-bottom": "10px"
         }
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader-32cd2df9.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/InfoHeader-32cd2df9.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -24,58 +24,58 @@
     F as I,
     z as M,
     ah as R,
     aa as z,
     S as Q,
     aj as W,
     O as X
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     a as Z,
     L as ee
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     _ as N,
     V as te,
     g as j
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
 import {
     g as ae,
     a as ie
-} from "./ListviewItem-2bd74fad.js";
+} from "./ListviewItem-e2342ce8.js";
 import {
     b as oe,
     a as D
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     b as re,
     V as g,
     a as B,
     c as le,
     d as ne
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     a as se,
     i as me,
     V as c,
     l as P,
     k as de
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     b as ue,
     V as pe
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     b as ye,
     c as fe
-} from "./layout-b0232ef9.js";
+} from "./layout-ff13c6fd.js";
 import {
     V as ge,
     a as ce
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 const ve = U({
         ...se(),
         ...ye()
     }, "VLayout"),
     S = E()({
         name: "VLayout",
         props: ve(),
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing-7290acd0.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ItemsListing-7290acd0.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,281 +1,278 @@
 import {
-    _ as ye,
-    L as he,
+    _ as be,
+    L as ye,
     i as ke,
     s as we
-} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
+} from "./ListviewItem-e2342ce8.js"; /* empty css                             */
 import {
-    p as Ce,
-    m as Ve,
-    as as Se,
-    g as _e,
+    p as Se,
+    m as Ce,
+    as as Ve,
+    g as Ie,
     f as $e,
-    d as Ie,
-    r as g,
+    d as Be,
+    r as h,
     w as z,
-    o as j,
-    j as r,
-    k as N,
-    at as Me,
-    au as Ae,
+    o as G,
+    j as c,
+    k as A,
+    at as _e,
+    au as Me,
     q as m,
-    y as I,
-    Y as U,
-    M as y,
+    y as N,
+    Y as j,
+    M as g,
     L as O,
-    N as F,
+    N as B,
     n as le,
-    a5 as Ne,
-    a6 as Fe,
-    l as Le,
-    O as Pe,
-    I as Be,
+    a5 as Ae,
+    a6 as Ne,
+    l as Fe,
+    O as Le,
+    I as Pe,
     b as Oe,
     x as d,
     B as b,
-    v as $,
-    F as Q,
-    z as X,
-    A as Z,
-    K,
-    W as ze,
-    D as w
-} from "./index-ade73b84.js";
+    K as D,
+    A as K,
+    v as w,
+    F as X,
+    z as Z,
+    D as y,
+    W as ze
+} from "./index-a5bb9833.js";
 import {
     _ as Ee
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
 import {
     C as Te,
     L as De
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     A as x
-} from "./Alert-4d78da02.js";
+} from "./Alert-a5ce795e.js";
 import {
     a as ee
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as Re
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
-    V as qe
-} from "./VSpacer-159b0383.js";
+    o as qe,
+    p as Ke,
+    c as He,
+    q as Ue,
+    r as je,
+    s as Ge,
+    v as We,
+    g as Ye,
+    i as Je,
+    w as Qe,
+    x as Xe,
+    l as L,
+    V as R,
+    k as Ze
+} from "./VBtn-629f5316.js";
 import {
-    o as Ke,
-    p as He,
-    c as Ue,
-    q as je,
-    r as Ge,
-    s as We,
-    v as Ye,
-    g as Je,
-    i as Qe,
-    w as Xe,
-    x as Ze,
-    l as P,
-    V as D,
-    k as xe
-} from "./VBtn-61e39030.js";
+    V as xe
+} from "./VBadge-f7d58168.js";
 import {
-    V as et
-} from "./VBadge-12aff0c7.js";
-import {
-    m as tt,
-    a as at,
+    m as et,
+    a as tt,
     c as te,
-    f as ot,
-    V as lt,
-    b as nt
-} from "./VMenu-ccc026f2.js";
+    f as at,
+    V as ot,
+    b as lt
+} from "./VMenu-240a4406.js";
 import {
     V as ae
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
-    V as it
-} from "./VSelect-a66ffc02.js";
+    V as nt
+} from "./VSelect-4d69c543.js";
 import {
-    V as st,
-    a as rt
-} from "./VRow-74a0e5a5.js";
-const ut = Ce({
+    V as it,
+    a as st
+} from "./VRow-7d86481a.js";
+const rt = Se({
         multiLine: Boolean,
         timeout: {
             type: [Number, String],
             default: 5e3
         },
         vertical: Boolean,
-        ...Ke({
+        ...qe({
             location: "bottom"
         }),
+        ...Ke(),
         ...He(),
         ...Ue(),
-        ...je(),
-        ...Ve(),
-        ...Se(tt({
+        ...Ce(),
+        ...Ve(et({
             transition: "v-snackbar-transition"
         }), ["persistent", "noClickAnimation", "scrim", "scrollStrategy"])
     }, "VSnackbar"),
-    ct = _e()({
+    ut = Ie()({
         name: "VSnackbar",
-        props: ut(),
+        props: rt(),
         emits: {
             "update:modelValue": a => !0
         },
-        setup(a, p) {
+        setup(a, f) {
             let {
                 slots: t
-            } = p;
+            } = f;
             const s = $e(a, "modelValue"),
                 {
                     locationStyles: C
-                } = Ge(a),
+                } = je(a),
                 {
                     positionClasses: v
-                } = We(a),
+                } = Ge(a),
                 {
                     scopeId: n
-                } = at(),
+                } = tt(),
                 {
-                    themeClasses: S
-                } = Ie(a),
+                    themeClasses: I
+                } = Be(a),
                 {
-                    colorClasses: L,
+                    colorClasses: F,
                     colorStyles: V,
-                    variantClasses: _
-                } = Ye(a),
+                    variantClasses: $
+                } = We(a),
                 {
                     roundedClasses: l
-                } = Je(a),
-                o = g();
-            z(s, f), z(() => a.timeout, f), j(() => {
-                s.value && f()
+                } = Ye(a),
+                o = h();
+            z(s, p), z(() => a.timeout, p), G(() => {
+                s.value && p()
             });
-            let k = -1;
+            let S = -1;
 
-            function f() {
-                window.clearTimeout(k);
-                const c = Number(a.timeout);
-                !s.value || c === -1 || (k = window.setTimeout(() => {
+            function p() {
+                window.clearTimeout(S);
+                const u = Number(a.timeout);
+                !s.value || u === -1 || (S = window.setTimeout(() => {
                     s.value = !1
-                }, c))
+                }, u))
             }
 
-            function h() {
-                window.clearTimeout(k)
+            function k() {
+                window.clearTimeout(S)
             }
-            return Qe(() => {
-                const [c] = te.filterProps(a);
-                return r(te, N({
+            return Je(() => {
+                const [u] = te.filterProps(a);
+                return c(te, A({
                     ref: o,
                     class: ["v-snackbar", {
                         "v-snackbar--active": s.value,
                         "v-snackbar--multi-line": a.multiLine && !a.vertical,
                         "v-snackbar--vertical": a.vertical
                     }, v.value, a.class],
                     style: a.style
-                }, c, {
+                }, u, {
                     modelValue: s.value,
-                    "onUpdate:modelValue": M => s.value = M,
-                    contentProps: N({
-                        class: ["v-snackbar__wrapper", S.value, L.value, l.value, _.value],
+                    "onUpdate:modelValue": _ => s.value = _,
+                    contentProps: A({
+                        class: ["v-snackbar__wrapper", I.value, F.value, l.value, $.value],
                         style: [C.value, V.value],
-                        onPointerenter: h,
-                        onPointerleave: f
-                    }, c.contentProps),
+                        onPointerenter: k,
+                        onPointerleave: p
+                    }, u.contentProps),
                     persistent: !0,
                     noClickAnimation: !0,
                     scrim: !1,
                     scrollStrategy: "none",
                     _disableGlobalStack: !0
                 }, n), {
-                    default: () => [Xe(!1, "v-snackbar"), t.default && r("div", {
+                    default: () => [Qe(!1, "v-snackbar"), t.default && c("div", {
                         class: "v-snackbar__content",
                         role: "status",
                         "aria-live": "polite"
-                    }, [t.default()]), t.actions && r(Ze, {
+                    }, [t.default()]), t.actions && c(Xe, {
                         defaults: {
                             VBtn: {
                                 variant: "text",
                                 ripple: !1
                             }
                         }
                     }, {
-                        default: () => [r("div", {
+                        default: () => [c("div", {
                             class: "v-snackbar__actions"
                         }, [t.actions()])]
                     })],
                     activator: t.activator
                 })
-            }), ot({}, o)
+            }), at({}, o)
         }
     }),
-    ne = (a, p) => {
+    ne = (a, f) => {
         const t = a.__vccOpts || a;
-        for (const [s, C] of p) t[s] = C;
+        for (const [s, C] of f) t[s] = C;
         return t
     },
-    dt = {},
-    mt = a => (Ne("data-v-259be2b2"), a = a(), Fe(), a),
-    vt = {
+    ct = {},
+    dt = a => (Ae("data-v-259be2b2"), a = a(), Ne(), a),
+    mt = {
         class: "container"
     },
-    ft = mt(() => O("div", {
+    vt = dt(() => O("div", {
         class: "spinner"
     }, null, -1)),
-    pt = [ft];
+    pt = [vt];
 
-function gt(a, p) {
-    return m(), I("div", vt, pt)
+function ft(a, f) {
+    return m(), N("div", mt, pt)
 }
-const bt = ne(dt, [
-        ["render", gt],
+const ht = ne(ct, [
+        ["render", ft],
         ["__scopeId", "data-v-259be2b2"],
         ["__file", "/home/oumoussa/side-projects/infinite/src/components/Spinner.vue"]
     ]),
-    yt = a => ({
+    gt = a => ({
         loading() {
             a.value = "loading"
         },
         loaded() {
             a.value = "loaded"
         },
         complete() {
             a.value = "complete"
         },
         error() {
             a.value = "error"
         }
     }),
-    ht = (a, p, t) => () => {
+    bt = (a, f, t) => () => {
         const s = t.parentEl || document.documentElement;
-        t.prevHeight = s.scrollHeight, p.loading(), a("infinite", p)
+        t.prevHeight = s.scrollHeight, f.loading(), a("infinite", f)
     },
-    kt = (a, p) => {
+    yt = (a, f) => {
         const t = a.getBoundingClientRect();
-        if (!p) return t.top >= 0 && t.bottom <= window.innerHeight;
-        const s = p.getBoundingClientRect();
+        if (!f) return t.top >= 0 && t.bottom <= window.innerHeight;
+        const s = f.getBoundingClientRect();
         return t.top >= s.top && t.bottom <= s.bottom
     },
     oe = a => {
         a.parentEl = document.querySelector(a.target) || null;
-        let p = `0px 0px ${a.distance}px 0px`;
-        a.top && (p = `${a.distance}px 0px 0px 0px`);
+        let f = `0px 0px ${a.distance}px 0px`;
+        a.top && (f = `${a.distance}px 0px 0px 0px`);
         const t = new IntersectionObserver(s => {
             s[0].isIntersecting && (a.firstload && a.emit(), a.firstload = !0)
         }, {
             root: a.parentEl,
-            rootMargin: p
+            rootMargin: f
         });
         return t.observe(a.infiniteLoading.value), t
     },
-    wt = {
+    kt = {
         class: "state-error"
     },
-    Ct = {
+    wt = {
         __name: "InfiniteLoading",
         props: {
             top: {
                 type: Boolean,
                 required: !1
             },
             target: {
@@ -298,129 +295,126 @@
             slots: {
                 type: Object,
                 required: !1
             }
         },
         emits: ["infinite"],
         setup(a, {
-            emit: p
+            emit: f
         }) {
             const t = a;
             let s = null;
-            const C = g(null),
-                v = g("ready"),
+            const C = h(null),
+                v = h("ready"),
                 {
                     top: n,
-                    firstload: S,
-                    target: L,
+                    firstload: I,
+                    target: F,
                     distance: V
                 } = t,
                 {
-                    identifier: _
-                } = Me(t),
+                    identifier: $
+                } = _e(t),
                 l = {
                     infiniteLoading: C,
-                    target: L,
+                    target: F,
                     top: n,
-                    firstload: S,
+                    firstload: I,
                     distance: V,
                     prevHeight: 0,
                     parentEl: null
                 };
-            l.emit = ht(p, yt(v), l);
-            const o = () => z(v, async f => {
-                    const h = l.parentEl || document.documentElement;
-                    await le(), f == "loaded" && n && (h.scrollTop = h.scrollHeight - l.prevHeight), f == "loaded" && kt(C.value, l.parentEl) && l.emit(), f == "complete" && s.disconnect()
+            l.emit = bt(f, gt(v), l);
+            const o = () => z(v, async p => {
+                    const k = l.parentEl || document.documentElement;
+                    await le(), p == "loaded" && n && (k.scrollTop = k.scrollHeight - l.prevHeight), p == "loaded" && yt(C.value, l.parentEl) && l.emit(), p == "complete" && s.disconnect()
                 }),
-                k = () => z(_, () => {
+                S = () => z($, () => {
                     v.value = "ready", s.disconnect(), s = oe(l)
                 });
-            return j(() => {
-                s = oe(l), o(), _ && k()
-            }), Ae(() => {
+            return G(() => {
+                s = oe(l), o(), $ && S()
+            }), Me(() => {
                 s.disconnect()
-            }), (f, h) => (m(), I("div", {
+            }), (p, k) => (m(), N("div", {
                 ref_key: "infiniteLoading",
                 ref: C
-            }, [v.value == "loading" ? U(f.$slots, "spinner", {
+            }, [v.value == "loading" ? j(p.$slots, "spinner", {
                 key: 0
-            }, () => [r(bt)], !0) : y("v-if", !0), v.value == "complete" ? U(f.$slots, "complete", {
+            }, () => [c(ht)], !0) : g("v-if", !0), v.value == "complete" ? j(p.$slots, "complete", {
                 key: 1
             }, () => {
-                var c;
-                return [O("span", null, F(((c = a.slots) == null ? void 0 : c.complete) || "No more results!"), 1)]
-            }, !0) : y("v-if", !0), v.value == "error" ? U(f.$slots, "error", {
+                var u;
+                return [O("span", null, B(((u = a.slots) == null ? void 0 : u.complete) || "No more results!"), 1)]
+            }, !0) : g("v-if", !0), v.value == "error" ? j(p.$slots, "error", {
                 key: 2,
                 retry: l.emit
             }, () => {
-                var c;
-                return [O("span", wt, [O("span", null, F(((c = a.slots) == null ? void 0 : c.error) || "Oops something went wrong!"), 1), O("button", {
+                var u;
+                return [O("span", kt, [O("span", null, B(((u = a.slots) == null ? void 0 : u.error) || "Oops something went wrong!"), 1), O("button", {
                     class: "retry",
-                    onClick: h[0] || (h[0] = (...M) => l.emit && l.emit(...M))
+                    onClick: k[0] || (k[0] = (..._) => l.emit && l.emit(..._))
                 }, " retry ")])]
-            }, !0) : y("v-if", !0)], 512))
+            }, !0) : g("v-if", !0)], 512))
         }
     },
-    Vt = ne(Ct, [
+    St = ne(wt, [
         ["__scopeId", "data-v-9d82030b"],
         ["__file", "/home/oumoussa/side-projects/infinite/src/components/InfiniteLoading.vue"]
     ]);
-const St = {
-        key: 0
-    },
-    _t = {
+const Ct = {
         key: 0
     },
-    $t = {
+    Vt = {
         key: 2
     },
     It = {
         key: 3
     },
-    Mt = {
+    $t = {
         style: {
             height: "30px",
             "margin-top": "20px"
         }
     },
-    Ut = function(a, p, t, s, C, v = !0) {
-        var V, _;
+    qt = function(a, f, t, s, C, v = !0) {
+        var V, $;
         let n = [];
         if (C) {
             const l = C.toLowerCase();
-            for (const o of a)(o.name.toLowerCase().includes(l) || "artist" in o && ((V = o.artist) != null && V.name.toLowerCase().includes(l)) || "album" in o && ((_ = o.album) != null && _.name.toLowerCase().includes(l)) || "artists" in o && o.artists && o.artists[0].name.toLowerCase().includes(l)) && n.push(o)
+            for (const o of a)(o.name.toLowerCase().includes(l) || "artist" in o && ((V = o.artist) != null && V.name.toLowerCase().includes(l)) || "album" in o && (($ = o.album) != null && $.name.toLowerCase().includes(l)) || "artists" in o && o.artists && o.artists[0].name.toLowerCase().includes(l)) && n.push(o)
         } else n = a;
         s == "sort_name" && n.sort((l, o) => (l.sort_name || l.name).localeCompare(o.sort_name || o.name)), s == "sort_album" && n.sort((l, o) => {
-            var k, f;
-            return (f = l.album) == null ? void 0 : f.name.localeCompare((k = o.album) == null ? void 0 : k.name)
+            var S, p;
+            return (p = l.album) == null ? void 0 : p.name.localeCompare((S = o.album) == null ? void 0 : S.name)
         }), s == "sort_artist" && n.sort((l, o) => l.artists[0].name.localeCompare(o.artists[0].name)), s == "track_number" && (n.sort((l, o) => (l.track_number || 0) - (o.track_number || 0)), n.sort((l, o) => (l.disc_number || 0) - (o.disc_number || 0))), s == "position" && n.sort((l, o) => (l.position || 0) - (o.position || 0)), s == "position DESC" && n.sort((l, o) => (o.position || 0) - (l.position || 0)), s == "year" && n.sort((l, o) => (l.year || 0) - (o.year || 0)), s == "timestamp_added DESC" && n.sort((l, o) => (o.timestamp_added || 0) - (l.timestamp_added || 0)), s == "duration" && n.sort((l, o) => (l.duration || 0) - (o.duration || 0)), s == "provider" && n.sort((l, o) => l.provider.localeCompare(o.provider)), v && (n = n.filter(l => l.favorite));
-        const S = n.length,
-            L = n.slice(p, p + t);
+        const I = n.length,
+            F = n.slice(f, f + t);
         return {
-            items: L,
-            count: L.length,
+            items: F,
+            count: F.length,
             limit: t,
-            offset: p,
-            total: S
+            offset: f,
+            total: I
         }
     },
-    jt = Le({
+    Kt = Fe({
         __name: "ItemsListing",
         props: {
             itemtype: {},
             sortKeys: {
                 default: () => ["sort_name", "timestamp_added DESC"]
             },
             showTrackNumber: {
                 type: Boolean,
                 default: !0
             },
             showProvider: {
                 type: Boolean,
-                default: Object.keys(Pe.providers).length > 1
+                default: Object.keys(Le.providers).length > 1
             },
             showAlbum: {
                 type: Boolean,
                 default: !0
             },
             showMenu: {
                 type: Boolean,
@@ -436,14 +430,26 @@
             },
             parentItem: {
                 default: void 0
             },
             showAlbumArtistsOnlyFilter: {
                 type: Boolean
             },
+            showSearchButton: {
+                type: Boolean,
+                default: void 0
+            },
+            showRefreshButton: {
+                type: Boolean,
+                default: void 0
+            },
+            showSelectButton: {
+                type: Boolean,
+                default: void 0
+            },
             updateAvailable: {
                 type: Boolean
             },
             title: {},
             hideOnEmpty: {
                 type: Boolean,
                 default: !1
@@ -451,448 +457,454 @@
             checksum: {
                 default: void 0
             },
             loadData: {}
         },
         emits: ["refreshClicked"],
         setup(a, {
-            emit: p
+            emit: f
         }) {
             const t = a,
                 s = 100,
-                C = Be(),
-                v = g("list"),
-                n = g(""),
-                S = g("sort_name"),
-                L = g(!1),
-                V = g(!1),
-                _ = g(!1),
-                l = g(0),
-                o = g([]),
-                k = g(),
-                f = g(!1),
-                h = g(!1),
-                c = g([]),
-                M = g(!1),
-                ie = g(!1),
-                E = g(!1),
-                T = g(!0),
+                C = Pe(),
+                v = h("list"),
+                n = h(""),
+                I = h("sort_name"),
+                F = h(!1),
+                V = h(!1),
+                $ = h(!1),
+                l = h(0),
+                o = h([]),
+                S = h(),
+                p = h(!1),
+                k = h(!1),
+                u = h([]),
+                _ = h(!1),
+                ie = h(!1),
+                E = h(!1),
+                T = h(!0),
                 se = function() {
                     V.value ? V.value = !1 : (V.value = !0, le(() => {
                         var e;
                         (e = document.getElementById("searchInput")) == null || e.focus()
                     }))
                 },
                 re = function(e) {
-                    return w({
+                    return y({
                         breakpoint: "bp1",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 2 : w({
+                    }) ? 2 : y({
                         breakpoint: "bp1",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
-                    }) && w({
+                    }) && y({
                         breakpoint: "bp4",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 3 : w({
+                    }) ? 3 : y({
                         breakpoint: "bp4",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
-                    }) && w({
+                    }) && y({
                         breakpoint: "bp6",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 4 : w({
+                    }) ? 4 : y({
                         breakpoint: "bp6",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
-                    }) && w({
+                    }) && y({
                         breakpoint: "bp7",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 5 : w({
+                    }) ? 5 : y({
                         breakpoint: "bp7",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
-                    }) && w({
+                    }) && y({
                         breakpoint: "bp8",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 6 : w({
+                    }) ? 6 : y({
                         breakpoint: "bp8",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
-                    }) && w({
+                    }) && y({
                         breakpoint: "bp9",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 7 : w({
+                    }) ? 7 : y({
                         breakpoint: "bp9",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
-                    }) && w({
+                    }) && y({
                         breakpoint: "bp10",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
-                    }) ? 8 : w({
+                    }) ? 8 : y({
                         breakpoint: "bp10",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
                     }) ? 9 : 0
                 },
                 ue = function() {
                     v.value === "panel" ? v.value = "list" : v.value = "panel", localStorage.setItem(`viewMode.${t.itemtype}`, v.value)
                 },
                 ce = function() {
-                    h.value = !h.value;
-                    const e = h.value ? "true" : "false";
-                    localStorage.setItem(`favoriteFilter.${t.itemtype}`, e), A(!0)
+                    k.value = !k.value;
+                    const e = k.value ? "true" : "false";
+                    localStorage.setItem(`favoriteFilter.${t.itemtype}`, e), M(!0)
                 },
                 de = function() {
                     T.value = !T.value;
                     const e = T.value ? "true" : "false";
-                    localStorage.setItem(`albumArtistsFilter.${t.itemtype}`, e), A(!0)
+                    localStorage.setItem(`albumArtistsFilter.${t.itemtype}`, e), M(!0)
                 },
-                G = function(e) {
-                    return c.value.includes(e)
+                W = function(e) {
+                    return u.value.includes(e)
                 },
-                W = function(e, u) {
-                    if (u) c.value.includes(e) || c.value.push(e);
+                Y = function(e, r) {
+                    if (r) u.value.includes(e) || u.value.push(e);
                     else
-                        for (let i = 0; i < c.value.length; i++) c.value[i] === e && c.value.splice(i, 1);
-                    b.blockGlobalPlayMenu = c.value.length > 0
+                        for (let i = 0; i < u.value.length; i++) u.value[i] === e && u.value.splice(i, 1);
+                    b.blockGlobalPlayMenu = u.value.length > 0
                 },
                 me = function() {
-                    c.value = [], E.value = !1, b.blockGlobalPlayMenu = !1
+                    u.value = [], E.value = !1, b.blockGlobalPlayMenu = !1
                 },
-                H = function() {
-                    c.value.length > 0 ? M.value = !0 : E.value = !E.value
+                U = function() {
+                    u.value.length > 0 ? _.value = !0 : E.value = !E.value
                 },
                 ve = function(e) {
-                    A(!0)
+                    M(!0)
                 },
-                q = function(e) {
-                    c.value = [e], M.value = !0
+                H = function(e) {
+                    u.value = [e], _.value = !0
                 },
-                fe = function() {
-                    A(!0), p("refreshClicked")
+                pe = function() {
+                    M(!0), f("refreshClicked")
                 },
-                Y = function(e) {
-                    var u;
+                J = function(e) {
+                    var r;
                     if (!ke(e)) {
-                        q(e);
+                        H(e);
                         return
-                    } ["artist", "album", "playlist"].includes(e.media_type) || !((u = b.selectedPlayer) != null && u.available) ? C.push({
+                    } ["artist", "album", "playlist"].includes(e.media_type) || !((r = b.selectedPlayer) != null && r.available) ? C.push({
                         name: e.media_type,
                         params: {
                             itemId: e.item_id,
                             provider: e.provider
                         }
-                    }) : q(e)
+                    }) : H(e)
                 },
-                pe = function(e, u) {
-                    e !== void 0 && (S.value = e), localStorage.setItem(`sortBy.${t.itemtype}`, S.value), A(!0)
+                fe = function(e, r) {
+                    e !== void 0 && (I.value = e), localStorage.setItem(`sortBy.${t.itemtype}`, I.value), M(!0)
                 },
-                ge = function(e) {
+                he = function(e) {
                     if (o.value.length == 0) {
                         e.loaded();
                         return
                     }
-                    if (k.value !== void 0 && l.value >= k.value) {
+                    if (S.value !== void 0 && l.value >= S.value) {
                         e.loaded();
                         return
                     }
-                    l.value += s, A().then(() => {
+                    l.value += s, M().then(() => {
                         e.loaded()
                     })
                 },
-                be = function() {
+                ge = function() {
                     localStorage.setItem("globalsearch", n.value), C.push({
                         name: "search",
                         params: {
                             initSearch: n.value
                         }
                     })
                 };
             z(() => n.value, e => {
-                e && (V.value = !0), A(!0)
+                e && (V.value = !0), M(!0)
             }), z(() => t.updateAvailable, e => {
-                e && o.value.length == 0 && A(!0)
+                e && o.value.length == 0 && M(!0)
             }), z(() => t.checksum, e => {
-                e && A(!0)
+                e && M(!0)
             });
-            const A = async function(e = !1, u = s) {
-                e && (l.value = 0, ie.value = !1), f.value = !0;
-                const i = await t.loadData(l.value, u, S.value, n.value || "", h.value, T.value);
-                l.value ? o.value.push(...i.items) : o.value = i.items, k.value = i.total, f.value = !1;
-                let B = `search.${t.itemtype}`;
-                t.parentItem && (B += t.parentItem.item_id), localStorage.setItem(B, n.value)
+            const M = async function(e = !1, r = s) {
+                e && (l.value = 0, ie.value = !1), p.value = !0;
+                const i = await t.loadData(l.value, r, I.value, n.value || "", k.value, T.value);
+                l.value ? o.value.push(...i.items) : o.value = i.items, S.value = i.total, p.value = !1;
+                let P = `search.${t.itemtype}`;
+                t.parentItem && (P += t.parentItem.item_id), localStorage.setItem(P, n.value)
             };
-            j(() => {
+            G(() => {
                 const e = localStorage.getItem(`viewMode.${t.itemtype}`);
                 e && e !== "null" ? v.value = e : t.itemtype == "artists" || t.itemtype == "albums" ? v.value = "panel" : v.value = "list";
-                const u = localStorage.getItem(`sortBy.${t.itemtype}`);
-                if (u && u !== "null" ? S.value = u : S.value = t.sortKeys[0], t.showFavoritesOnlyFilter !== !1) {
-                    const R = localStorage.getItem(`favoriteFilter.${t.itemtype}`);
-                    R && R == "true" && (h.value = !0)
+                const r = localStorage.getItem(`sortBy.${t.itemtype}`);
+                if (r && r !== "null" ? I.value = r : I.value = t.sortKeys[0], t.showFavoritesOnlyFilter !== !1) {
+                    const q = localStorage.getItem(`favoriteFilter.${t.itemtype}`);
+                    q && q == "true" && (k.value = !0)
                 }
                 if (t.showAlbumArtistsOnlyFilter !== !1) {
-                    const R = localStorage.getItem(`albumArtistsFilter.${t.itemtype}`);
-                    R && (T.value = R == "true")
+                    const q = localStorage.getItem(`albumArtistsFilter.${t.itemtype}`);
+                    q && (T.value = q == "true")
                 }
                 let i = `search.${t.itemtype}`;
                 t.parentItem && (i += t.parentItem.item_id);
-                const B = localStorage.getItem(i);
-                B && B !== "null" && (console.log("savedSearch", B), n.value = B), A(!0)
+                const P = localStorage.getItem(i);
+                P && P !== "null" && (console.log("savedSearch", P), n.value = P), M(!0)
             });
-            const J = function(e) {
-                M.value || (e.key === "a" && (e.ctrlKey || e.metaKey) ? (e.preventDefault(), c.value = o.value) : !_.value && e.key == "Backspace" ? n.value = n.value.slice(0, -1) : !_.value && e.key.length == 1 && (n.value += e.key, V.value = !0))
+            const Q = function(e) {
+                _.value || (e.key === "a" && (e.ctrlKey || e.metaKey) ? (e.preventDefault(), u.value = o.value) : !$.value && e.key == "Backspace" ? n.value = n.value.slice(0, -1) : !$.value && e.key.length == 1 && (n.value += e.key, V.value = !0))
             };
-            return document.addEventListener("keydown", J), Oe(() => {
-                document.removeEventListener("keydown", J)
-            }), (e, u) => e.hideOnEmpty && o.value.length == 0 ? y("", !0) : (m(), I("section", St, [r(ye, {
-                modelValue: M.value,
-                "onUpdate:modelValue": u[0] || (u[0] = i => M.value = i),
-                items: c.value,
+            return document.addEventListener("keydown", Q), Oe(() => {
+                document.removeEventListener("keydown", Q)
+            }), (e, r) => e.hideOnEmpty && o.value.length == 0 ? g("", !0) : (m(), N("section", Ct, [c(be, {
+                modelValue: _.value,
+                "onUpdate:modelValue": r[0] || (r[0] = i => _.value = i),
+                items: u.value,
                 "parent-item": e.parentItem,
                 onClear: me,
                 onDelete: ve
-            }, null, 8, ["modelValue", "items", "parent-item"]), r(ee, null, {
-                default: d(() => [r(Re, {
+            }, null, 8, ["modelValue", "items", "parent-item"]), c(ee, null, {
+                default: d(() => [c(Re, {
                     density: "compact",
                     variant: "flat",
                     color: "transparent"
                 }, {
-                    title: d(() => [!e.$vuetify.display.mobile && e.title ? (m(), I("span", _t, F(e.title), 1)) : y("", !0)]),
-                    default: d(() => [r(qe), r(P, N(t, {
+                    title: d(() => [D(B(e.title), 1)]),
+                    append: d(() => [(e.showSelectButton != null ? e.showSelectButton : K(y)("bp1") || !e.title) ? (m(), w(L, A({
+                        key: 0
+                    }, t, {
                         icon: E.value ? "mdi-checkbox-multiple-outline" : "mdi-checkbox-multiple-blank-outline",
                         variant: "plain",
-                        onClick: H,
+                        onClick: U,
                         title: e.$t("tooltip.select_items")
-                    }), null, 16, ["icon", "title"]), e.showFavoritesOnlyFilter !== !1 ? (m(), $(P, N({
-                        key: 0
+                    }), null, 16, ["icon", "title"])) : g("", !0), D(" " + B(e.showSelectButton) + " ", 1), e.showFavoritesOnlyFilter !== !1 ? (m(), w(L, A({
+                        key: 1
                     }, t, {
                         icon: "",
                         variant: "plain",
                         onClick: ce,
                         title: e.$t("tooltip.filter_favorites")
                     }), {
-                        default: d(() => [r(D, {
-                            icon: h.value ? "mdi-heart" : "mdi-heart-outline"
+                        default: d(() => [c(R, {
+                            icon: k.value ? "mdi-heart" : "mdi-heart-outline"
                         }, null, 8, ["icon"])]),
                         _: 1
-                    }, 16, ["title"])) : y("", !0), e.showAlbumArtistsOnlyFilter ? (m(), $(P, N({
-                        key: 1
+                    }, 16, ["title"])) : g("", !0), e.showAlbumArtistsOnlyFilter ? (m(), w(L, A({
+                        key: 2
                     }, t, {
                         icon: "",
                         variant: "plain",
                         onClick: de,
                         title: e.$t("tooltip.album_artist_filter")
                     }), {
-                        default: d(() => [r(D, {
+                        default: d(() => [c(R, {
                             icon: T.value ? "mdi-account-music" : "mdi-account-music-outline"
                         }, null, 8, ["icon"])]),
                         _: 1
-                    }, 16, ["title"])) : y("", !0), r(P, N(t, {
+                    }, 16, ["title"])) : g("", !0), (e.showRefreshButton != null ? e.showRefreshButton : K(y)("bp1") || !e.title) ? (m(), w(L, A({
+                        key: 3
+                    }, t, {
                         icon: "",
                         variant: "plain",
-                        onClick: u[1] || (u[1] = i => fe()),
+                        onClick: r[1] || (r[1] = i => pe()),
                         title: e.updateAvailable ? e.$t("tooltip.refresh_new_content") : e.$t("tooltip.refresh")
                     }), {
-                        default: d(() => [r(et, {
+                        default: d(() => [c(xe, {
                             "model-value": e.updateAvailable,
                             color: "error",
                             dot: ""
                         }, {
-                            default: d(() => [r(D, {
+                            default: d(() => [c(R, {
                                 icon: "mdi-refresh"
                             })]),
                             _: 1
                         }, 8, ["model-value"])]),
                         _: 1
-                    }, 16, ["title"]), e.sortKeys.length > 1 ? (m(), $(nt, {
-                        key: 2,
-                        modelValue: L.value,
-                        "onUpdate:modelValue": u[2] || (u[2] = i => L.value = i),
+                    }, 16, ["title"])) : g("", !0), e.sortKeys.length > 1 ? (m(), w(lt, {
+                        key: 4,
+                        modelValue: F.value,
+                        "onUpdate:modelValue": r[2] || (r[2] = i => F.value = i),
                         location: "bottom end",
                         "close-on-content-click": !0
                     }, {
                         activator: d(({
                             props: i
-                        }) => [r(P, N({
+                        }) => [c(L, A({
                             icon: ""
                         }, i, {
                             variant: "plain",
                             title: e.$t("tooltip.sort_options")
                         }), {
-                            default: d(() => [r(D, N(i, {
+                            default: d(() => [c(R, A(i, {
                                 icon: "mdi-sort"
                             }), null, 16)]),
                             _: 2
                         }, 1040, ["title"])]),
-                        default: d(() => [r(ee, null, {
-                            default: d(() => [r(lt, null, {
-                                default: d(() => [(m(!0), I(Q, null, X(e.sortKeys, i => (m(), I("div", {
+                        default: d(() => [c(ee, null, {
+                            default: d(() => [c(ot, null, {
+                                default: d(() => [(m(!0), N(X, null, Z(e.sortKeys, i => (m(), N("div", {
                                     key: i
-                                }, [r(De, {
-                                    onClick: B => pe(i)
+                                }, [c(De, {
+                                    onClick: P => fe(i)
                                 }, {
-                                    title: d(() => [K(F(e.$t("sort." + i)), 1)]),
-                                    append: d(() => [S.value == i ? (m(), $(D, {
+                                    title: d(() => [D(B(e.$t("sort." + i)), 1)]),
+                                    append: d(() => [I.value == i ? (m(), w(R, {
                                         key: 0,
                                         icon: "mdi-check"
-                                    })) : y("", !0)]),
+                                    })) : g("", !0)]),
                                     _: 2
-                                }, 1032, ["onClick"]), r(ae)]))), 128))]),
+                                }, 1032, ["onClick"]), c(ae)]))), 128))]),
                                 _: 1
                             })]),
                             _: 1
                         })]),
                         _: 1
-                    }, 8, ["modelValue"])) : y("", !0), r(P, N(t, {
+                    }, 8, ["modelValue"])) : g("", !0), (e.showSearchButton != null ? e.showSearchButton : K(y)("bp1") || !e.title) ? (m(), w(L, A({
+                        key: 5
+                    }, t, {
                         icon: "",
                         variant: "plain",
-                        onClick: u[3] || (u[3] = i => se()),
+                        onClick: r[3] || (r[3] = i => se()),
                         title: e.$t("tooltip.search")
                     }), {
-                        default: d(() => [r(D, {
+                        default: d(() => [c(R, {
                             icon: "mdi-magnify"
                         })]),
                         _: 1
-                    }, 16, ["title"]), r(P, N(t, {
+                    }, 16, ["title"])) : g("", !0), c(L, A(t, {
                         icon: v.value == "panel" ? "mdi-view-list" : "mdi-grid",
                         variant: "plain",
-                        onClick: u[4] || (u[4] = i => ue()),
+                        onClick: r[4] || (r[4] = i => ue()),
                         title: e.$t("tooltip.toggle_view_mode")
                     }), null, 16, ["icon", "title"])]),
                     _: 1
-                }), r(ae), V.value ? (m(), $(it, {
+                }), c(ae), V.value ? (m(), w(nt, {
                     key: 0,
                     id: "searchInput",
                     modelValue: n.value,
-                    "onUpdate:modelValue": u[5] || (u[5] = i => n.value = i),
+                    "onUpdate:modelValue": r[5] || (r[5] = i => n.value = i),
                     clearable: "",
                     "prepend-inner-icon": "mdi-magnify",
                     label: e.$t("search"),
                     "hide-details": "",
                     variant: "filled",
                     style: {
                         width: "auto",
                         "margin-left": "15px",
                         "margin-right": "15px",
                         "margin-top": "10px"
                     },
-                    onFocus: u[6] || (u[6] = i => _.value = !0),
-                    onBlur: u[7] || (u[7] = i => _.value = !1)
-                }, null, 8, ["modelValue", "label"])) : y("", !0), r(Te, null, {
-                    default: d(() => [f.value ? (m(), $(xe, {
+                    onFocus: r[6] || (r[6] = i => $.value = !0),
+                    onBlur: r[7] || (r[7] = i => $.value = !1)
+                }, null, 8, ["modelValue", "label"])) : g("", !0), c(Te, null, {
+                    default: d(() => [p.value ? (m(), w(Ze, {
                         key: 0,
                         indeterminate: ""
-                    })) : y("", !0), v.value == "panel" ? (m(), $(st, {
+                    })) : g("", !0), v.value == "panel" ? (m(), w(it, {
                         key: 1
                     }, {
-                        default: d(() => [(m(!0), I(Q, null, X(o.value, i => (m(), $(rt, {
+                        default: d(() => [(m(!0), N(X, null, Z(o.value, i => (m(), w(st, {
                             key: i.uri,
                             class: ze(`col-${re(e.$vuetify.display.width)}`)
                         }, {
-                            default: d(() => [r(Ee, {
+                            default: d(() => [c(Ee, {
                                 item: i,
-                                "is-selected": G(i),
+                                "is-selected": W(i),
                                 "show-checkboxes": E.value,
                                 "show-track-number": e.showTrackNumber,
-                                onSelect: W,
-                                onMenu: q,
-                                onClick: Y
+                                onSelect: Y,
+                                onMenu: H,
+                                onClick: J
                             }, null, 8, ["item", "is-selected", "show-checkboxes", "show-track-number"])]),
                             _: 2
                         }, 1032, ["class"]))), 128))]),
                         _: 1
-                    })) : y("", !0), v.value == "list" ? (m(), I("div", $t, [r(Z(we), {
+                    })) : g("", !0), v.value == "list" ? (m(), N("div", Vt, [c(K(we), {
                         items: o.value,
                         "item-size": 70,
                         "key-field": "uri",
                         "page-mode": ""
                     }, {
                         default: d(({
                             item: i
-                        }) => [(m(), $(he, {
+                        }) => [(m(), w(ye, {
                             key: i.uri,
                             item: i,
                             "show-track-number": e.showTrackNumber,
                             "show-disc-number": e.showTrackNumber,
                             "show-duration": e.showDuration,
                             "show-favorite": e.showFavoritesOnlyFilter,
                             "show-menu": e.showMenu,
                             "show-provider": e.showProvider,
                             "show-album": e.showAlbum,
                             "show-checkboxes": E.value,
-                            "is-selected": G(i),
+                            "is-selected": W(i),
                             "show-details": e.itemtype.includes("versions"),
                             "parent-item": e.parentItem,
-                            onSelect: W,
-                            onMenu: q,
-                            onClick: Y
+                            onSelect: Y,
+                            onMenu: H,
+                            onClick: J
                         }, null, 8, ["item", "show-track-number", "show-disc-number", "show-duration", "show-favorite", "show-menu", "show-provider", "show-album", "show-checkboxes", "is-selected", "show-details", "parent-item"]))]),
                         _: 1
-                    }, 8, ["items"])])) : y("", !0), r(Z(Vt), {
-                        onInfinite: ge
-                    }), !f.value && o.value.length == 0 ? (m(), I("div", It, [!f.value && o.value.length == 0 && (n.value || h.value) ? (m(), $(x, {
+                    }, 8, ["items"])])) : g("", !0), c(K(St), {
+                        onInfinite: he
+                    }), !p.value && o.value.length == 0 ? (m(), N("div", It, [!p.value && o.value.length == 0 && (n.value || k.value) ? (m(), w(x, {
                         key: 0,
                         title: e.$t("no_content_filter")
                     }, {
-                        default: d(() => [n.value ? (m(), $(P, {
+                        default: d(() => [n.value ? (m(), w(L, {
                             key: 0,
                             style: {
                                 "margin-top": "15px"
                             },
-                            onClick: be
+                            onClick: ge
                         }, {
-                            default: d(() => [K(F(e.$t("try_global_search")), 1)]),
+                            default: d(() => [D(B(e.$t("try_global_search")), 1)]),
                             _: 1
-                        })) : y("", !0)]),
+                        })) : g("", !0)]),
                         _: 1
-                    }, 8, ["title"])) : !f.value && o.value.length == 0 ? (m(), $(x, {
+                    }, 8, ["title"])) : !p.value && o.value.length == 0 ? (m(), w(x, {
                         key: 1
                     }, {
-                        default: d(() => [K(F(e.$t("no_content")), 1)]),
+                        default: d(() => [D(B(e.$t("no_content")), 1)]),
                         _: 1
-                    })) : y("", !0)])) : y("", !0), r(ct, {
-                        "model-value": c.value.length > 1,
+                    })) : g("", !0)])) : g("", !0), c(ut, {
+                        "model-value": u.value.length > 1,
                         timeout: -1,
                         style: {
                             "margin-bottom": "120px"
                         }
                     }, {
-                        actions: d(() => [r(P, {
+                        actions: d(() => [c(L, {
                             color: "primary",
                             variant: "text",
-                            onClick: u[8] || (u[8] = i => M.value = !0)
+                            onClick: r[8] || (r[8] = i => _.value = !0)
                         }, {
-                            default: d(() => [K(F(e.$t("actions")), 1)]),
+                            default: d(() => [D(B(e.$t("actions")), 1)]),
                             _: 1
                         })]),
-                        default: d(() => [O("span", null, F(e.$t("items_selected", [c.value.length])), 1)]),
+                        default: d(() => [O("span", null, B(e.$t("items_selected", [u.value.length])), 1)]),
                         _: 1
-                    }, 8, ["model-value"]), O("div", Mt, [!c.value.length && k.value ? (m(), I("span", {
+                    }, 8, ["model-value"]), O("div", $t, [!u.value.length && S.value ? (m(), N("span", {
                         key: 0,
                         style: {
                             cursor: "pointer"
                         },
-                        onClick: H
-                    }, F(e.$t("items_total", [k.value])), 1)) : c.value.length ? (m(), I("span", {
+                        onClick: U
+                    }, B(e.$t("items_total", [S.value])), 1)) : u.value.length ? (m(), N("span", {
                         key: 1,
                         style: {
                             cursor: "pointer"
                         },
-                        onClick: H
-                    }, F(e.$t("items_selected", [c.value.length])), 1)) : y("", !0)])]),
+                        onClick: U
+                    }, B(e.$t("items_selected", [u.value.length])), 1)) : g("", !0)])]),
                     _: 1
                 })]),
                 _: 1
             })]))
         }
     });
 export {
-    jt as _, Ut as f
+    Kt as _, qt as f
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryAlbums-757b8aa2.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryAlbums-55bc0ec5.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -6,35 +6,34 @@
     O as r,
     S as v,
     b as n,
     o as y,
     af as s,
     q as E,
     v as D
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as M
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
-import "./VListItem-f848c028.js";
-import "./Container-282a676b.js"; /* empty css              */
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js";
-const F = d({
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
+import "./VListItem-39677d21.js";
+import "./Container-4773c160.js"; /* empty css              */
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js";
+const z = d({
     __name: "LibraryAlbums",
     setup(A) {
         const {
             t: p
         } = f(), l = i([]), o = i(!1);
         m.topBarContextMenuItems = [{
             label: "sync_now",
@@ -64,10 +63,10 @@
             "load-data": u,
             "sort-keys": ["sort_name", "timestamp_added DESC", "sort_artist", "year"],
             "update-available": o.value
         }, null, 8, ["items", "update-available"]))
     }
 });
 export {
-    F as
+    z as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryArtists-225ce0c1.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryArtists-0afc0ed9.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -6,35 +6,34 @@
     O as o,
     S as y,
     b as m,
     o as E,
     af as s,
     q as I,
     v as A
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as D
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
-import "./VListItem-f848c028.js";
-import "./Container-282a676b.js"; /* empty css              */
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js";
-const F = d({
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
+import "./VListItem-39677d21.js";
+import "./Container-4773c160.js"; /* empty css              */
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js";
+const z = d({
     __name: "LibraryArtists",
     setup(M) {
         const {
             t: p
         } = v(), l = i([]), r = i(!1), u = async function(t, a, e, c, _ = !0, f = !0) {
             const b = _ || void 0;
             return r.value = !1, await o.getLibraryArtists(b, c, a, t, e, f)
@@ -62,10 +61,10 @@
             "load-data": u,
             "show-album-artists-only-filter": !0,
             "update-available": r.value
         }, null, 8, ["items", "update-available"]))
     }
 });
 export {
-    F as
+    z as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryPlaylists-4ffdc19f.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryPlaylists-86c14bd9.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -7,35 +7,34 @@
     S as b,
     ag as E,
     b as p,
     o as I,
     af as i,
     q as A,
     v as D
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as M
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
-import "./VListItem-f848c028.js";
-import "./Container-282a676b.js"; /* empty css              */
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js";
-const z = y({
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
+import "./VListItem-39677d21.js";
+import "./Container-4773c160.js"; /* empty css              */
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js";
+const W = y({
     __name: "LibraryPlaylists",
     setup(T) {
         const {
             t: n
         } = v(), m = l([]), s = l(!1);
         r.topBarContextMenuItems = [{
             label: "sync_now",
@@ -82,10 +81,10 @@
             "sort-keys": ["sort_name", "timestamp_added DESC"],
             "update-available": s.value,
             onRefreshClicked: t[0] || (t[0] = a => s.value = !1)
         }, null, 8, ["items", "update-available"]))
     }
 });
 export {
-    z as
+    W as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryRadios-a948d358.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryRadios-3bd5ccff.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -6,35 +6,34 @@
     O as o,
     S as l,
     b as p,
     o as I,
     af as i,
     q as D,
     v as E
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as A
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
-import "./VListItem-f848c028.js";
-import "./Container-282a676b.js"; /* empty css              */
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js";
-const F = v({
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
+import "./VListItem-39677d21.js";
+import "./Container-4773c160.js"; /* empty css              */
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js";
+const z = v({
     __name: "LibraryRadios",
     setup(M) {
         const {
             t: s
         } = y(), u = n([]), r = n(!1);
         m.topBarContextMenuItems = [{
             label: "sync_now",
@@ -78,10 +77,10 @@
             "load-data": c,
             "sort-keys": ["sort_name", "timestamp_added DESC"],
             "update-available": r.value
         }, null, 8, ["items", "update-available"]))
     }
 });
 export {
-    F as
+    z as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryTracks-5a540fa3.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/LibraryTracks-07ab288b.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -6,35 +6,34 @@
     O as r,
     S as l,
     b as p,
     o as E,
     af as n,
     q as I,
     v as T
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as D
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
-import "./VListItem-f848c028.js";
-import "./Container-282a676b.js"; /* empty css              */
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js";
-const z = v({
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
+import "./VListItem-39677d21.js";
+import "./Container-4773c160.js"; /* empty css              */
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js";
+const $ = v({
     __name: "LibraryTracks",
     setup(k) {
         const {
             t: s
         } = y(), c = i([]), o = i(!1);
         m.topBarContextMenuItems = [{
             label: "sync_now",
@@ -79,10 +78,10 @@
             "sort-keys": ["sort_name", "timestamp_added DESC", "sort_artist", "duration"],
             "show-album": !1,
             "update-available": o.value
         }, null, 8, ["items", "update-available"]))
     }
 });
 export {
-    z as
+    $ as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-2bd74fad.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ListviewItem-e2342ce8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -49,67 +49,67 @@
     ah as Y,
     ae as ut,
     aj as dt,
     a7 as ie,
     D as ae,
     U as ct,
     aA as se
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as De,
     V as Ie,
     d as mt
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
 import {
     L as Q,
     a as fe,
     _ as ft
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as pt,
     b as Ve
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     i as ht,
     a as yt,
     z as vt,
     d as bt,
     A as gt,
     B as _t,
     C as St,
     l as ne,
     V as U
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     V as wt
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     c as ue,
     a as kt
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     m as It,
     a as $e,
     b as Vt,
     V as $t
-} from "./VSelect-a66ffc02.js";
+} from "./VSelect-4d69c543.js";
 import {
     V as de
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     d as zt,
     a as ze,
     b as At
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     m as Tt,
     u as Ct,
     c as Ae,
     V as Pt
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 
 function Mt() {
     var e = window.navigator.userAgent,
         t = e.indexOf("MSIE ");
     if (t > 0) return parseInt(e.substring(t + 5, e.indexOf(".", t)), 10);
     var i = e.indexOf("Trident/");
     if (i > 0) {
@@ -1662,12 +1662,12 @@
                 }, 8, ["disabled", "context-menu-items"])), [
                     [o, () => t("menu", s.item)]
                 ])])
             }
         }
     });
 const Ui = ft(Ai, [
-    ["__scopeId", "data-v-d473232c"]
+    ["__scopeId", "data-v-3ecb0dd0"]
 ]);
 export {
     Ui as L, ri as V, Ni as _, mi as a, oi as b, q as c, We as g, G as i, je as s
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-732a7603.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/ListviewItem-707ff3c9.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.v-checkbox .v-selection-control{min-height:var(--v-input-control-height)}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}div.v-slide-group__next{position:absolute;right:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}div.v-slide-group__prev{position:absolute;left:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.content-spacing{display:flex;flex-flow:column;gap:10px}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.flicking-viewport{position:relative;overflow:hidden}.flicking-viewport.vertical{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex}.flicking-viewport.vertical>.flicking-camera{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}.flicking-viewport.flicking-hidden>.flicking-camera>*{visibility:hidden}.flicking-camera{width:100%;height:100%;display:-webkit-box;display:-ms-flexbox;display:flex;position:relative;-webkit-box-orient:horizontal;-webkit-box-direction:normal;-ms-flex-direction:row;flex-direction:row;z-index:1;will-change:transform}.flicking-camera>*{-ms-flex-negative:0;flex-shrink:0}.v-item-group{flex:0 1 auto;max-width:100%;position:relative;transition:.2s cubic-bezier(.4,0,.2,1)}.fullscreen-menu .v-overlay__content{left:0px;right:0px;top:0px;bottom:0px}.hiresicon[data-v-d473232c],.hiresicondark[data-v-d473232c]{margin-top:5px;margin-right:15px;margin-left:15px;filter:invert(100%)}
+@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.v-checkbox .v-selection-control{min-height:var(--v-input-control-height)}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}div.v-slide-group__next{position:absolute;right:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}div.v-slide-group__prev{position:absolute;left:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.content-spacing{display:flex;flex-flow:column;gap:10px}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.flicking-viewport{position:relative;overflow:hidden}.flicking-viewport.vertical{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex}.flicking-viewport.vertical>.flicking-camera{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}.flicking-viewport.flicking-hidden>.flicking-camera>*{visibility:hidden}.flicking-camera{width:100%;height:100%;display:-webkit-box;display:-ms-flexbox;display:flex;position:relative;-webkit-box-orient:horizontal;-webkit-box-direction:normal;-ms-flex-direction:row;flex-direction:row;z-index:1;will-change:transform}.flicking-camera>*{-ms-flex-negative:0;flex-shrink:0}.v-item-group{flex:0 1 auto;max-width:100%;position:relative;transition:.2s cubic-bezier(.4,0,.2,1)}.fullscreen-menu .v-overlay__content{left:0px;right:0px;top:0px;bottom:0px}.hiresicon[data-v-3ecb0dd0]{margin-top:5px;margin-right:15px;margin-left:15px;filter:invert(100%)}.hiresicondark[data-v-3ecb0dd0]{margin-top:5px;margin-right:15px;margin-left:15px}
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     m as P,
     a as U,
     c as O,
     f as X,
     V as L,
     b as T
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     p as V,
     as as Z,
     g as x,
     f as G,
     al as K,
     c as l,
@@ -29,36 +29,36 @@
     y as C,
     aA as f,
     O as R,
     B as J,
     ax as Q,
     w as W,
     aa as z
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     i as j,
     j as q
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     a as _
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     a as $
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 import {
     V as ee,
     c as te,
     b as ie
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     V as ae
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     a as Ae
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 const re = V({
         id: String,
         text: String,
         ...Z(P({
             closeOnBack: !1,
             location: "end",
             locationStrategy: "connected",
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -13,42 +13,42 @@
     N as r,
     A as f,
     a7 as S,
     aj as N,
     W as T,
     ah as A,
     aA as d
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as B,
     d as D,
     V as _
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
 import {
     L
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     c as F
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     V as M,
     b as z,
     c as p
-} from "./ListviewItem-2bd74fad.js";
+} from "./ListviewItem-e2342ce8.js";
 import {
     c as H,
     d as b,
     b as j
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     V as c
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     a as P
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 const J = C({
     __name: "PanelviewItem",
     props: {
         item: {},
         size: {
             default: 200
         },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlayerQueue-7ca94b07.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PlayerQueue-6206a6c6.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -20,58 +20,58 @@
     L as v,
     M as _,
     A as V,
     k as J,
     ah as h,
     a2 as ue,
     S as ae
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     L as oe,
     s as ie
-} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
+} from "./ListviewItem-e2342ce8.js"; /* empty css                             */
 import {
     C as ne,
     L as g
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     A as O
-} from "./Alert-4d78da02.js";
+} from "./Alert-a5ce795e.js";
 import {
     V as P,
     a as se
-} from "./VTabs-21d8affa.js";
+} from "./VTabs-f388999c.js";
 import {
     V as F
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
 import {
     l as A,
     V as q
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     a as re,
     c as de
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as me,
     b as G
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as pe
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     a as y
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     V as C
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as ve
-} from "./VDialog-93a2100b.js";
-import "./VSelect-a66ffc02.js"; /* empty css              */
+} from "./VDialog-667c0916.js";
+import "./VSelect-4d69c543.js"; /* empty css              */
 const fe = v("br", null, null, -1),
     _e = {
         key: 0
     },
     be = {
         key: 0
     },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Players-5c99fe5e.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Players-73f88aa0.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -15,29 +15,29 @@
     F as x,
     Q as I,
     A as d,
     j as p,
     L as m,
     N as _,
     M as F
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     C as M,
     L as T,
     a as z
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     B as b
-} from "./Button-4a781169.js";
+} from "./Button-00834c6c.js";
 import {
     V as f
-} from "./VBtn-61e39030.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VListItem-f848c028.js"; /* empty css              */
+} from "./VBtn-629f5316.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VListItem-39677d21.js"; /* empty css              */
 const O = {
         class: "line-clamp-1"
     },
     R = {
         class: "line-clamp-1"
     },
     K = w({
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlaylistDetails-f8a1c191.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/PlaylistDetails-ad67ce68.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,47 +1,46 @@
 import {
     _,
     f as y
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
 import {
     _ as k
-} from "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js";
+} from "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js";
 import {
     C as b
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     l as h,
     r as c,
     w,
     o as I,
     O as l,
     af as D,
     b as C,
     q as E,
     y as g,
     j as n,
     x as T
-} from "./index-ade73b84.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VMenu-ccc026f2.js";
-import "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
-import "./VListItem-f848c028.js";
-import "./VDialog-93a2100b.js";
-import "./VCard-f3e11b51.js";
-import "./VToolbar-806969a3.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js"; /* empty css              */
-import "./layout-b0232ef9.js";
-const W = h({
+} from "./index-a5bb9833.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VMenu-240a4406.js";
+import "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
+import "./VListItem-39677d21.js";
+import "./VDialog-667c0916.js";
+import "./VCard-04ae357c.js";
+import "./VToolbar-b79315e8.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js"; /* empty css              */
+import "./layout-ff13c6fd.js";
+const Q = h({
     __name: "PlaylistDetails",
     props: {
         itemId: {},
         provider: {}
     },
     setup(d) {
         const i = d,
@@ -91,10 +90,10 @@
                 }, null, 8, ["parent-item", "update-available", "title"])]),
                 _: 1
             })])
         }
     }
 });
 export {
-    W as
+    Q as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Providers-65d3d824.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Providers-0fb3a52e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -22,44 +22,44 @@
     N as u,
     k as H,
     K as m,
     M as v,
     Q as J,
     a5 as W,
     a6 as X
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     C as I,
     L as A,
     a as S,
     _ as Y
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     B as b
-} from "./Button-4a781169.js";
+} from "./Button-00834c6c.js";
 import {
     A as Z
-} from "./Alert-4d78da02.js";
+} from "./Alert-a5ce795e.js";
 import {
     a as B
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     V as ee
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     b as te
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     l as ne,
     V as g
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     V as ae
-} from "./VDivider-adefbf87.js";
-import "./VListItem-f848c028.js"; /* empty css              */
+} from "./VDivider-df9414f0.js";
+import "./VListItem-39677d21.js"; /* empty css              */
 const ie = _ => (W("data-v-273ae240"), _ = _(), X(), _),
     se = {
         class: "line-clamp-1"
     },
     oe = ie(() => p("br", null, null, -1)),
     re = {
         class: "line-clamp-1"
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/RadioDetails-71dc877e.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/RadioDetails-fb9a6d90.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -13,68 +13,67 @@
     L as B,
     O as m,
     ai as D,
     K as h,
     N as u,
     A as R,
     ah as T
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as x,
     f as z
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
 import {
     _ as F
-} from "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js";
+} from "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js";
 import {
     C as V,
     L as S,
     a as j
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as q
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as A
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     V as E
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 import {
     a as K
-} from "./VCard-f3e11b51.js";
+} from "./VCard-04ae357c.js";
 import {
     l as O
-} from "./VBtn-61e39030.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js"; /* empty css              */
-import "./layout-b0232ef9.js";
+} from "./VBtn-629f5316.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js"; /* empty css              */
+import "./layout-ff13c6fd.js";
 const P = B("br", null, null, -1),
-    ue = C({
+    pe = C({
         __name: "RadioDetails",
         props: {
             itemId: {},
             provider: {}
         },
-        setup(w) {
-            const o = w,
+        setup(y) {
+            const o = y,
                 a = g(),
-                y = async function() {
+                w = async function() {
                     a.value = await m.getRadio(o.itemId, o.provider)
                 };
             L(() => o.itemId, e => {
-                e && y()
+                e && w()
             }, {
                 immediate: !0
             });
             const k = async function(e, c, n, t, f = !0) {
                 const d = [];
                 if (o.provider == "library") {
                     const l = await m.getRadioVersions(o.itemId, o.provider);
@@ -116,37 +115,39 @@
                         style: {
                             height: "55px"
                         }
                     }, null, 8, ["title"]), i(A), i(V, null, {
                         default: r(() => [i(E, null, {
                             default: r(() => {
                                 var n;
-                                return [(s(!0), _(N, null, $((n = a.value) == null ? void 0 : n.provider_mappings, t => (s(), p(S, null, {
+                                return [(s(!0), _(N, null, $((n = a.value) == null ? void 0 : n.provider_mappings, t => (s(), p(S, {
+                                    key: t.provider_instance
+                                }, {
                                     prepend: r(() => [i(j, {
                                         domain: t.provider_domain,
                                         size: 30
                                     }, null, 8, ["domain"])]),
                                     title: r(() => [h(u(R(m).providerManifests[t.provider_domain].name), 1)]),
                                     subtitle: r(() => [h(u(t.item_id) + " | " + u(t.audio_format.content_type) + " bits ", 1)]),
                                     append: r(() => [t.url ? (s(), p(O, {
                                         key: 0,
                                         variant: "plain",
                                         icon: "mdi-open-in-new",
                                         onClick: T(f => b(t.url), ["prevent"])
                                     }, null, 8, ["onClick"])) : v("", !0)]),
                                     _: 2
-                                }, 1024))), 256))]
+                                }, 1024))), 128))]
                             }),
                             _: 1
                         })]),
                         _: 1
                     })]),
                     _: 1
                 })) : v("", !0)]),
                 _: 1
             })]))
         }
     });
 export {
-    ue as
+    pe as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Search-f31ee239.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Search-1975e9f7.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     _ as q,
     L as A,
     s as G
-} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
+} from "./ListviewItem-e2342ce8.js"; /* empty css                             */
 import {
     l as H,
     I as O,
     e as W,
     r as i,
     c as w,
     w as L,
@@ -24,49 +24,49 @@
     A as X,
     N as _,
     k as Y,
     B as P,
     O as T,
     K as Z,
     W as z
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     _ as ee
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
 import {
     C as te
-} from "./Container-282a676b.js";
+} from "./Container-4773c160.js";
 import {
     V as ae
-} from "./VSelect-a66ffc02.js";
+} from "./VSelect-4d69c543.js";
 import {
     b as le,
     a as se
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 import {
     V as re,
     a as oe
-} from "./VRow-74a0e5a5.js";
+} from "./VRow-7d86481a.js";
 import {
     V as ue
-} from "./VToolbar-806969a3.js";
+} from "./VToolbar-b79315e8.js";
 import {
     V as ie
-} from "./VSpacer-159b0383.js";
+} from "./VSpacer-82874439.js";
 import {
     V as ne
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
 import {
     l as ve,
     k as me
-} from "./VBtn-61e39030.js";
-import "./VDivider-adefbf87.js";
-import "./VCard-f3e11b51.js";
-import "./VListItem-f848c028.js";
-import "./VMenu-ccc026f2.js"; /* empty css              */
+} from "./VBtn-629f5316.js";
+import "./VDivider-df9414f0.js";
+import "./VCard-04ae357c.js";
+import "./VListItem-39677d21.js";
+import "./VMenu-240a4406.js"; /* empty css              */
 const fe = {
         key: 2
     },
     ce = {
         style: {
             "margin-left": "15px"
         }
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Settings-f159e60c.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/Settings-05fc67af.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,23 +8,23 @@
     j as e,
     x as a,
     K as o,
     N as s,
     T as g,
     v as y,
     R as V
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     V as n,
     a as T
-} from "./VTabs-21d8affa.js";
+} from "./VTabs-f388999c.js";
 import {
     V as b
-} from "./VDivider-adefbf87.js";
-import "./VBtn-61e39030.js";
+} from "./VDivider-df9414f0.js";
+import "./VBtn-629f5316.js";
 const B = m({
     __name: "Settings",
     setup(C) {
         const i = d(),
             u = v(() => {
                 var t, r;
                 return (t = i.currentRoute.value.name) != null && t.toString().includes("player") ? "players" : (r = i.currentRoute.value.name) != null && r.toString().includes("core") ? "core" : "providers"
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/TrackDetails-ca02e9b2.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/TrackDetails-3d9e1c6f.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,203 +1,206 @@
 import {
-    l as E,
+    l as U,
     r as b,
-    w as U,
-    o as z,
+    w as z,
+    o as R,
     O as l,
-    af as R,
-    b as F,
-    q as p,
-    y as w,
+    af as F,
+    b as P,
+    q as d,
+    y as k,
     j as s,
     x as m,
-    v as k,
-    F as P,
-    z as S,
-    M as y,
-    L as h,
-    ai as V,
-    K as I,
+    v as h,
+    F as S,
+    z as j,
+    M as w,
+    L as A,
+    ai as y,
+    K as V,
     N as c,
-    A as j,
-    ah as q
-} from "./index-ade73b84.js";
+    A as I,
+    D as q,
+    ah as H
+} from "./index-a5bb9833.js";
 import {
     _ as T,
     f as $
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js";
 import {
-    _ as H
-} from "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js";
+    _ as K
+} from "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js";
 import {
     C,
-    L as K,
-    a as O
-} from "./Container-282a676b.js";
-import {
-    V as G
-} from "./VToolbar-806969a3.js";
+    L as O,
+    a as G
+} from "./Container-4773c160.js";
 import {
     V as J
-} from "./VDivider-adefbf87.js";
+} from "./VToolbar-b79315e8.js";
 import {
-    V as M
-} from "./VMenu-ccc026f2.js";
+    V as Q
+} from "./VDivider-df9414f0.js";
 import {
-    a as Q
-} from "./VCard-f3e11b51.js";
+    V as W
+} from "./VMenu-240a4406.js";
 import {
-    l as W
-} from "./VBtn-61e39030.js";
-import "./ListviewItem-2bd74fad.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
-import "./VDialog-93a2100b.js";
-import "./VListItem-f848c028.js";
-import "./VSelect-a66ffc02.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
-import "./Alert-4d78da02.js";
-import "./VSpacer-159b0383.js";
-import "./VBadge-12aff0c7.js";
-import "./VRow-74a0e5a5.js"; /* empty css              */
-import "./layout-b0232ef9.js";
-const X = h("br", null, null, -1),
-    Y = h("br", null, null, -1),
-    Z = ["src"],
-    ye = E({
+    a as X
+} from "./VCard-04ae357c.js";
+import {
+    l as Y
+} from "./VBtn-629f5316.js";
+import "./ListviewItem-e2342ce8.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js";
+import "./VDialog-667c0916.js";
+import "./VListItem-39677d21.js";
+import "./VSelect-4d69c543.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js";
+import "./Alert-a5ce795e.js";
+import "./VBadge-f7d58168.js";
+import "./VRow-7d86481a.js"; /* empty css              */
+import "./layout-ff13c6fd.js";
+const Z = A("br", null, null, -1),
+    M = A("br", null, null, -1),
+    x = ["src"],
+    ye = U({
         __name: "TrackDetails",
         props: {
             itemId: {},
             provider: {},
             album: {}
         },
-        setup(A) {
-            const a = A,
-                D = b(""),
-                d = b(!1),
+        setup(D) {
+            const a = D,
+                g = b(""),
+                p = b(!1),
                 n = b(),
                 f = async function() {
-                    console.log("props", a), n.value = await l.getTrack(a.itemId, a.provider, a.album), D.value = "versions"
+                    console.log("props", a), n.value = await l.getTrack(a.itemId, a.provider, a.album), g.value = "versions"
                 };
-            U(() => a.itemId, e => {
+            z(() => a.itemId, e => {
                 e && f()
             }, {
                 immediate: !0
-            }), z(() => {
-                const e = l.subscribe(R.MEDIA_ITEM_ADDED, r => {
+            }), R(() => {
+                const e = l.subscribe(F.MEDIA_ITEM_ADDED, r => {
                     var t;
                     const o = r.data;
-                    ((t = n.value) == null ? void 0 : t.uri) == o.uri && (d.value = !0)
+                    ((t = n.value) == null ? void 0 : t.uri) == o.uri && (p.value = !0)
                 });
-                F(e)
+                P(e)
             });
-            const g = async function(e, r, o, t, v = !0) {
+            const B = async function(e, r, o, t, v = !0) {
                 const u = [];
                 if (a.provider == "library") {
                     const i = await l.getTrackVersions(a.itemId, a.provider);
                     u.push(...i)
                 }
-                for (const i of V(n.value)) {
+                for (const i of y(n.value)) {
                     const _ = await l.getTrackVersions(i.item_id, i.provider_instance);
                     u.push(..._)
                 }
                 return $(u, e, r, o, t, v)
-            }, B = async function(e, r, o, t, v = !0) {
+            }, L = async function(e, r, o, t, v = !0) {
                 const u = [];
                 if (a.provider == "library") {
                     const i = await l.getTrackAlbums(a.itemId, a.provider);
                     u.push(...i)
                 }
-                for (const i of V(n.value)) {
+                for (const i of y(n.value)) {
                     const _ = await l.getTrackAlbums(i.item_id, i.provider_instance);
                     u.push(..._)
                 }
                 return $(u, e, r, o, t, v)
-            }, L = function(e) {
+            }, N = function(e) {
                 window.open(e, "_blank")
-            }, N = function(e, r) {
+            }, E = function(e, r) {
                 return `${l.baseUrl}/preview?provider=${e}&item_id=${encodeURIComponent(r)}`
             };
-            return (e, r) => (p(), w("section", null, [s(H, {
+            return (e, r) => (d(), k("section", null, [s(K, {
                 item: n.value,
                 "active-provider": e.provider
             }, null, 8, ["item", "active-provider"]), s(C, null, {
                 default: m(() => [s(T, {
                     itemtype: "trackalbums",
                     "parent-item": n.value,
                     "show-provider": !0,
                     "show-favorites-only-filter": !1,
                     "show-library": !0,
                     "show-track-number": !1,
-                    "load-data": B,
+                    "load-data": L,
                     "sort-keys": ["provider", "sort_name", "duration"],
-                    "update-available": d.value,
+                    "update-available": p.value,
                     onRefreshClicked: r[0] || (r[0] = o => {
-                        f(), d.value = !1
+                        f(), p.value = !1
                     }),
                     title: e.$t("appears_on"),
                     checksum: e.provider + e.itemId
-                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), X, s(T, {
+                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), Z, s(T, {
                     itemtype: "trackversions",
                     "parent-item": n.value,
                     "show-provider": !0,
                     "show-favorites-only-filter": !1,
                     "show-library": !0,
                     "show-track-number": !1,
-                    "load-data": g,
+                    "load-data": B,
                     "sort-keys": ["provider", "sort_name", "duration"],
-                    "update-available": d.value,
+                    "update-available": p.value,
                     onRefreshClicked: r[1] || (r[1] = o => {
-                        f(), d.value = !1
+                        f(), p.value = !1
                     }),
                     title: e.$t("other_versions"),
                     "hide-on-empty": !0,
                     checksum: e.provider + e.itemId
-                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), Y, e.provider == "library" ? (p(), k(Q, {
+                }, null, 8, ["parent-item", "update-available", "title", "checksum"]), M, e.provider == "library" ? (d(), h(X, {
                     key: 0,
                     style: {
                         "margin-bottom": "10px"
                     }
                 }, {
-                    default: m(() => [s(G, {
+                    default: m(() => [s(J, {
                         color: "transparent",
                         title: e.$t("mapped_providers"),
                         style: {
                             height: "55px"
                         }
-                    }, null, 8, ["title"]), s(J), s(C, null, {
-                        default: m(() => [s(M, null, {
+                    }, null, 8, ["title"]), s(Q), s(C, null, {
+                        default: m(() => [s(W, null, {
                             default: m(() => {
                                 var o;
-                                return [(p(!0), w(P, null, S((o = n.value) == null ? void 0 : o.provider_mappings, t => (p(), k(K, null, {
-                                    prepend: m(() => [s(O, {
+                                return [(d(!0), k(S, null, j((o = n.value) == null ? void 0 : o.provider_mappings, t => (d(), h(O, {
+                                    key: t.provider_instance
+                                }, {
+                                    prepend: m(() => [s(G, {
                                         domain: t.provider_domain,
                                         size: 30
                                     }, null, 8, ["domain"])]),
-                                    title: m(() => [I(c(j(l).providerManifests[t.provider_domain].name), 1)]),
-                                    subtitle: m(() => [I(c(t.item_id) + " | " + c(t.audio_format.content_type) + " | " + c(t.audio_format.sample_rate / 1e3) + "kHz/" + c(t.audio_format.bit_depth) + " bits ", 1)]),
-                                    append: m(() => [h("audio", {
+                                    title: m(() => [V(c(I(l).providerManifests[t.provider_domain].name), 1)]),
+                                    subtitle: m(() => [V(c(t.item_id) + " | " + c(t.audio_format.content_type) + " | " + c(t.audio_format.sample_rate / 1e3) + "kHz/" + c(t.audio_format.bit_depth) + " bits ", 1)]),
+                                    append: m(() => [I(q)("bp1") ? (d(), k("audio", {
+                                        key: 0,
                                         name: "preview",
                                         title: "preview",
                                         controls: "",
-                                        src: N(t.provider_domain, t.item_id)
-                                    }, null, 8, Z), t.url ? (p(), k(W, {
-                                        key: 0,
+                                        src: E(t.provider_domain, t.item_id)
+                                    }, null, 8, x)) : w("", !0), t.url ? (d(), h(Y, {
+                                        key: 1,
                                         variant: "plain",
                                         icon: "mdi-open-in-new",
-                                        onClick: q(v => L(t.url), ["prevent"])
-                                    }, null, 8, ["onClick"])) : y("", !0)]),
+                                        onClick: H(v => N(t.url), ["prevent"])
+                                    }, null, 8, ["onClick"])) : w("", !0)]),
                                     _: 2
-                                }, 1024))), 256))]
+                                }, 1024))), 128))]
                             }),
                             _: 1
                         })]),
                         _: 1
                     })]),
                     _: 1
-                })) : y("", !0)]),
+                })) : w("", !0)]),
                 _: 1
             })]))
         }
     });
 export {
     ye as
     default
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-12aff0c7.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBadge-f7d58168.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -7,31 +7,31 @@
     aw as P,
     ax as h,
     ay as T,
     j as t,
     Q as w,
     az as R,
     k as u
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     a as _,
     o as L,
     c as $,
     d as A,
     e as I,
     g as M,
     y as X,
     r as Y,
     i as j,
     V as z
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     m as D,
     M as F
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 const Q = B({
         bordered: Boolean,
         color: String,
         content: [Number, String],
         dot: Boolean,
         floating: Boolean,
         icon: S,
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-9c063078.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBadge-9c063078.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-61e39030.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBtn-629f5316.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -46,15 +46,15 @@
     s as bt,
     bb as yt,
     H as Ct,
     u as Le,
     T as pt,
     Q as St,
     a9 as kt
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 const Te = ["top", "bottom"],
     _t = ["start", "end", "left", "right"];
 
 function wt(e, t) {
     let [a, n] = e.split(" ");
     return n || (n = j(Te, a) ? "start" : j(_t, a) ? "top" : "center"), {
         side: Ce(a, t),
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-76f512af.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VBtn-76f512af.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-103d8462.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VCard-103d8462.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-f3e11b51.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VCard-04ae357c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,32 +22,32 @@
     I as ne,
     r as de,
     s as ie,
     g as se,
     O as le,
     L as ce,
     w as re
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     g as b,
     i as ue,
     j as n,
     p as P,
     av as u,
     m as ve,
     d as oe,
     c as V,
     Q as me,
     a9 as ge
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     e as p,
     a as A,
     b as ke
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 const ye = b()({
         name: "VCardActions",
         props: y(),
         setup(e, i) {
             let {
                 slots: t
             } = i;
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-28e4e64e.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDialog-28e4e64e.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-93a2100b.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDialog-667c0916.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -30,19 +30,19 @@
     b as be,
     o as ke,
     G as Z,
     n as ie,
     u as Ce,
     aL as Ie,
     aM as Se
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     f as Pe,
     e as Ae
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     a as T,
     z as Be,
     d as ue,
     q as oe,
     A as Me,
     i as O,
@@ -62,27 +62,27 @@
     N as Oe,
     C as Ge,
     O as Ke,
     w as Ne,
     V as F,
     x as z,
     y as Ue
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     a as ee,
     m as je,
     M as qe
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     m as He,
     i as Xe,
     a as Qe,
     c as ae,
     f as We
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 const de = Symbol.for("vuetify:v-chip-group"),
     Ye = A({
         column: Boolean,
         filter: Boolean,
         valueComparator: {
             type: Function,
             default: fe
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-adefbf87.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDivider-df9414f0.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,20 +7,20 @@
     ba as _,
     m as C,
     d as B,
     t as P,
     c as V,
     j as E,
     a as m
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     a as L,
     y as $,
     i as A
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 class y {
     constructor(r) {
         let {
             x: s,
             y: n,
             width: o,
             height: a
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-bc1524a3.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VDivider-bc1524a3.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-75456689.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VExpansionPanel-1ca09b07.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
     f as ze,
     F as Fe,
     k as Le,
     m as Re,
     d as Be,
     i as Me,
     av as re
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     c as fe,
     b as be,
     a as U,
     R as pe,
     y as Ne,
     i as q,
@@ -37,30 +37,30 @@
     e as J,
     z as Ae,
     d as ke,
     A as De,
     V as $e,
     B as Oe,
     C as je
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     d as qe,
     c as Ke
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     g as Ge,
     m as Ue,
     u as Qe,
     c as ue,
     f as Xe
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 import {
     d as Se,
     e as Ye
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 const le = Symbol.for("vuetify:v-slider");
 
 function We(e, a, t) {
     const l = t === "vertical",
         i = a.getBoundingClientRect(),
         m = "touches" in e ? e.touches[0] : e;
     return l ? m.clientY - (i.top + i.height / 2) : m.clientX - (i.left + i.width / 2)
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VGrid-b9c72806.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VGrid-b9c72806.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-b9e24cb0.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VListItem-b9e24cb0.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-f848c028.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VListItem-39677d21.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -18,15 +18,15 @@
     b as Ee,
     K as Fe,
     R as xe,
     O as Ge,
     u as He,
     f as We,
     x as le
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     g as M,
     aC as Ue,
     ba as qe,
     aD as be,
     ak as D,
     s as I,
@@ -52,15 +52,15 @@
     a as Ze,
     az as et,
     av as J,
     m as Ie,
     d as Ae,
     aX as re,
     bc as tt
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 
 function Pe(e) {
     let r = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : "div",
         a = arguments.length > 2 ? arguments[2] : void 0;
     return M()({
         name: a ?? Ue(qe(e.replace(/__/g, "-"))),
         props: {
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-b930657a.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VMenu-b930657a.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-ccc026f2.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VMenu-240a4406.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -44,37 +44,37 @@
     f as Je,
     u as Ot,
     b9 as kt,
     a9 as At,
     F as Lt,
     as as Vt,
     al as Tt
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     b as Z,
     g as Ft,
     s as ge,
     h as Bt,
     n as et,
     c as It,
     V as Dt,
     B as se,
     i as ke
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     u as Rt,
     f as Mt,
     g as _t,
     M as tt,
     h as nt,
     V as Ae,
     i as Nt,
     j as $t,
     m as Ht
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     a as re,
     d as Ce,
     i as J,
     x as ot,
     y as Wt,
     m as qt,
@@ -92,15 +92,15 @@
     P as Le,
     Q as le,
     S as ue,
     T as Ve,
     U as Te,
     h as Zt,
     W as Jt
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 const te = new WeakMap;
 
 function en(e, n) {
     Object.keys(n).forEach(t => {
         if (He(t)) {
             const o = We(t),
                 a = te.get(e);
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VRow-74a0e5a5.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VRow-7d86481a.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 /* empty css              */
 import {
     a as C,
     d as S
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     aB as i,
     aC as u,
     p as b,
     g as k,
     c as N,
     aD as j
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 const V = (() => i.reduce((t, a) => (t[a] = {
         type: [Boolean, String, Number],
         default: !1
     }, t), {}))(),
     v = (() => i.reduce((t, a) => {
         const e = "offset" + u(a);
         return t[e] = {
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-45a454b3.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VSelect-45a454b3.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-a66ffc02.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VSelect-4d69c543.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -39,22 +39,22 @@
     E as fe,
     am as Je,
     G as Qe,
     o as Ze,
     as as el,
     aw as ll,
     K as tl
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     e as nl,
     n as al,
     b as ol,
     s as il,
     f as ul
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     a as Q,
     E as sl,
     i as W,
     R as rl,
     V as re,
     F as cl,
@@ -65,40 +65,40 @@
     g as ml,
     e as yl,
     L as gl,
     n as _e,
     G as hl,
     H as Vl,
     x as bl
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     m as pe,
     M as Cl,
     I as xl,
     V as me
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 import {
     f as we,
     g as kl,
     u as Be,
     h as Il,
     m as Sl,
     c as ye,
     i as Pl,
     a as _l
-} from "./VDialog-93a2100b.js";
+} from "./VDialog-667c0916.js";
 import {
     f as Fe,
     g as pl,
     h as wl,
     i as Bl,
     j as Fl,
     b as Tl,
     V as Rl
-} from "./VMenu-ccc026f2.js";
+} from "./VMenu-240a4406.js";
 const Te = Symbol.for("vuetify:selection-control-group"),
     Re = O({
         color: String,
         disabled: {
             type: Boolean,
             default: null
         },
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-21d8affa.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VTabs-f388999c.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
     V as K,
     D as de,
     y as fe,
     l as J,
     E as me,
     F as ge,
     e as be
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     p as X,
     av as Q,
     g as Y,
     u as he,
     e as Se,
     s as k,
@@ -29,20 +29,20 @@
     as as Ce,
     r as Z,
     k as D,
     f as Te,
     t as T,
     i as ke,
     a as Ve
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     a as ee,
     b as we,
     s as Pe
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 
 function te(e) {
     const n = Math.abs(e);
     return Math.sign(e) * (n / ((1 / .501 - 2) * (1 - n) + 1))
 }
 
 function le(e) {
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-3cd3e980.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VTabs-3cd3e980.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-222d6375.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VToolbar-222d6375.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-806969a3.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/VToolbar-b79315e8.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -6,34 +6,34 @@
     b as I,
     c as E,
     e as D,
     u as w,
     f as $,
     g as j,
     x as u
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     p as V,
     g as k,
     j as a,
     m as F,
     t as U,
     d as q,
     u as z,
     s as A,
     c as h,
     i as G,
     a as o
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 import {
     c as J
-} from "./VDivider-adefbf87.js";
+} from "./VDivider-df9414f0.js";
 import {
     b as K
-} from "./VListItem-f848c028.js";
+} from "./VListItem-39677d21.js";
 const L = V({
         text: String,
         ...x(),
         ...y()
     }, "VToolbarTitle"),
     M = k()({
         name: "VToolbarTitle",
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_dark-75402cd0.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/cover_dark-75402cd0.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_light-b832ae9e.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/cover_light-b832ae9e.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/crossfade-ba51f69a.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/crossfade-ba51f69a.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/hires-438c7046.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/hires-438c7046.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ade73b84.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/index-a5bb9833.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -10452,133 +10452,133 @@
 }
 
 function $b() {
     return ke(ho)
 }
 const Eh = [{
         path: "/",
-        component: () => pe(() => import("./Default-4e51f0b8.js"), ["./Default-4e51f0b8.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./layout-b0232ef9.js", "./Button-4a781169.js", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-15e2fa72.css", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VExpansionPanel-75456689.js", "./VExpansionPanel-16e67e58.css", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./Default-8766b49d.css"], import.meta.url),
+        component: () => pe(() => import("./Default-7879cbcb.js"), ["./Default-7879cbcb.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./layout-ff13c6fd.js", "./Button-00834c6c.js", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-15e2fa72.css", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VExpansionPanel-1ca09b07.js", "./VExpansionPanel-16e67e58.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./Default-8766b49d.css"], import.meta.url),
         children: [{
             path: "",
             redirect: "/home",
             name: "homeredirect"
         }, {
             path: "/home",
             name: "home",
-            component: () => pe(() => import("./HomeView-af5707e7.js"), ["./HomeView-af5707e7.js", "./VRow-74a0e5a5.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VGrid-b9c72806.css", "./VCard-f3e11b51.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VCard-103d8462.css", "./HomeView-f559b858.css"], import.meta.url),
+            component: () => pe(() => import("./HomeView-95da878e.js"), ["./HomeView-95da878e.js", "./VRow-7d86481a.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VGrid-b9c72806.css", "./VCard-04ae357c.js", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VCard-103d8462.css", "./HomeView-f559b858.css"], import.meta.url),
             props: !0
         }, {
             path: "/search",
             name: "search",
-            component: () => pe(() => import("./Search-f31ee239.js"), ["./Search-f31ee239.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./VRow-74a0e5a5.js", "./VSpacer-159b0383.js", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./Search-1975e9f7.js"), ["./Search-1975e9f7.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./VRow-7d86481a.js", "./VSpacer-82874439.js", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/browse",
             name: "browse",
-            component: () => pe(() => import("./BrowseView-457188ac.js"), ["./BrowseView-457188ac.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./BrowseView-d5fa89c1.js"), ["./BrowseView-d5fa89c1.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: e => ({
                 path: e.query.path
             })
         }, {
             path: "/artists",
             name: "artists",
-            component: () => pe(() => import("./LibraryArtists-225ce0c1.js"), ["./LibraryArtists-225ce0c1.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryArtists-0afc0ed9.js"), ["./LibraryArtists-0afc0ed9.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/tracks",
             name: "tracks",
-            component: () => pe(() => import("./LibraryTracks-5a540fa3.js"), ["./LibraryTracks-5a540fa3.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryTracks-07ab288b.js"), ["./LibraryTracks-07ab288b.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/albums",
             name: "albums",
-            component: () => pe(() => import("./LibraryAlbums-757b8aa2.js"), ["./LibraryAlbums-757b8aa2.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryAlbums-55bc0ec5.js"), ["./LibraryAlbums-55bc0ec5.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/playlists",
             name: "playlists",
-            component: () => pe(() => import("./LibraryPlaylists-4ffdc19f.js"), ["./LibraryPlaylists-4ffdc19f.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryPlaylists-86c14bd9.js"), ["./LibraryPlaylists-86c14bd9.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/radios",
             name: "radios",
-            component: () => pe(() => import("./LibraryRadios-a948d358.js"), ["./LibraryRadios-a948d358.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryRadios-3bd5ccff.js"), ["./LibraryRadios-3bd5ccff.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/artists/:provider/:itemId",
             name: "artist",
-            component: () => pe(() => import("./ArtistDetails-7c7516d2.js"), ["./ArtistDetails-7c7516d2.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./ArtistDetails-cd5389ba.js"), ["./ArtistDetails-cd5389ba.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js", "./layout-ff13c6fd.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/albums/:provider/:itemId",
             name: "album",
-            component: () => pe(() => import("./AlbumDetails-55ac33a4.js"), ["./AlbumDetails-55ac33a4.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./AlbumDetails-ef8a3bee.js"), ["./AlbumDetails-ef8a3bee.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js", "./layout-ff13c6fd.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/tracks/:provider/:itemId",
             name: "track",
-            component: () => pe(() => import("./TrackDetails-ca02e9b2.js"), ["./TrackDetails-ca02e9b2.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./TrackDetails-3d9e1c6f.js"), ["./TrackDetails-3d9e1c6f.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js", "./layout-ff13c6fd.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: e => ({
                 ...e.params,
                 ...e.query
             })
         }, {
             path: "/radios/:provider/:itemId",
             name: "radio",
-            component: () => pe(() => import("./RadioDetails-71dc877e.js"), ["./RadioDetails-71dc877e.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./RadioDetails-fb9a6d90.js"), ["./RadioDetails-fb9a6d90.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js", "./layout-ff13c6fd.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/playlists/:provider/:itemId",
             name: "playlist",
-            component: () => pe(() => import("./PlaylistDetails-f8a1c191.js"), ["./PlaylistDetails-f8a1c191.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./PlaylistDetails-ad67ce68.js"), ["./PlaylistDetails-ad67ce68.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js", "./PanelviewItem-14a6b77a.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VBadge-f7d58168.js", "./VBadge-9c063078.css", "./VRow-7d86481a.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js", "./layout-ff13c6fd.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/playerqueue",
             name: "playerqueue",
-            component: () => pe(() => import("./PlayerQueue-7ca94b07.js"), ["./PlayerQueue-7ca94b07.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VTabs-21d8affa.js", "./VTabs-3cd3e980.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./PlayerQueue-6206a6c6.js"), ["./PlayerQueue-6206a6c6.js", "./ListviewItem-e2342ce8.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-4773c160.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-667c0916.js", "./VDialog-28e4e64e.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./ListviewItem-707ff3c9.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VTabs-f388999c.js", "./VTabs-3cd3e980.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/settings",
             name: "settings",
-            component: () => pe(() => import("./Settings-f159e60c.js"), ["./Settings-f159e60c.js", "./VTabs-21d8affa.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VTabs-3cd3e980.css"], import.meta.url),
+            component: () => pe(() => import("./Settings-05fc67af.js"), ["./Settings-05fc67af.js", "./VTabs-f388999c.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-df9414f0.js", "./VDivider-bc1524a3.css", "./VTabs-3cd3e980.css"], import.meta.url),
             props: !0,
             children: [{
                 path: "providers",
                 name: "providersettings",
-                component: () => pe(() => import("./Providers-65d3d824.js"), ["./Providers-65d3d824.js", "./Container-282a676b.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-4a781169.js", "./Button-15e2fa72.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./Providers-0e527c0c.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+                component: () => pe(() => import("./Providers-0fb3a52e.js"), ["./Providers-0fb3a52e.js", "./Container-4773c160.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-00834c6c.js", "./Button-15e2fa72.css", "./Alert-a5ce795e.js", "./Alert-c80b13d7.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./Providers-0e527c0c.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
                 props: !0
             }, {
                 path: "players",
                 name: "playersettings",
-                component: () => pe(() => import("./Players-5c99fe5e.js"), ["./Players-5c99fe5e.js", "./Container-282a676b.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-4a781169.js", "./Button-15e2fa72.css"], import.meta.url),
+                component: () => pe(() => import("./Players-73f88aa0.js"), ["./Players-73f88aa0.js", "./Container-4773c160.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-00834c6c.js", "./Button-15e2fa72.css"], import.meta.url),
                 props: !0
             }, {
                 path: "core",
                 name: "coresettings",
-                component: () => pe(() => import("./CoreConfigs-69940384.js"), ["./CoreConfigs-69940384.js", "./Container-282a676b.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./CoreConfigs-1c0e2549.css"], import.meta.url),
+                component: () => pe(() => import("./CoreConfigs-ec75d11a.js"), ["./CoreConfigs-ec75d11a.js", "./Container-4773c160.js", "./VMenu-240a4406.js", "./VDivider-df9414f0.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VToolbar-b79315e8.js", "./VToolbar-222d6375.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./CoreConfigs-1c0e2549.css"], import.meta.url),
                 props: !0
             }, {
                 path: "addprovider/:domain",
                 name: "addprovider",
-                component: () => pe(() => import("./AddProvider-a95ca786.js"), ["./AddProvider-a95ca786.js", "./index.browser-7e542916.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
+                component: () => pe(() => import("./AddProvider-fa211913.js"), ["./AddProvider-fa211913.js", "./index.browser-7e542916.js", "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js", "./VExpansionPanel-1ca09b07.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-df9414f0.js", "./VDivider-bc1524a3.css", "./VDialog-667c0916.js", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-240a4406.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./VSpacer-82874439.js", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editprovider/:instanceId",
                 name: "editprovider",
-                component: () => pe(() => import("./EditProvider-a2553a06.js"), ["./EditProvider-a2553a06.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
+                component: () => pe(() => import("./EditProvider-f88730fc.js"), ["./EditProvider-f88730fc.js", "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js", "./VExpansionPanel-1ca09b07.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-df9414f0.js", "./VDivider-bc1524a3.css", "./VDialog-667c0916.js", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-240a4406.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./VSpacer-82874439.js", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
                 props: !0
             }, {
                 path: "editplayer/:playerId",
                 name: "editplayer",
-                component: () => pe(() => import("./EditPlayer-f0c55a15.js"), ["./EditPlayer-f0c55a15.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
+                component: () => pe(() => import("./EditPlayer-33767eb3.js"), ["./EditPlayer-33767eb3.js", "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js", "./VExpansionPanel-1ca09b07.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-df9414f0.js", "./VDivider-bc1524a3.css", "./VDialog-667c0916.js", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-240a4406.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./VSpacer-82874439.js", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editcore/:domain",
                 name: "editcore",
-                component: () => pe(() => import("./EditCoreConfig-714d074a.js"), ["./EditCoreConfig-714d074a.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
+                component: () => pe(() => import("./EditCoreConfig-37eaad58.js"), ["./EditCoreConfig-37eaad58.js", "./EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js", "./VExpansionPanel-1ca09b07.js", "./VBtn-629f5316.js", "./VBtn-76f512af.css", "./VDivider-df9414f0.js", "./VDivider-bc1524a3.css", "./VDialog-667c0916.js", "./VListItem-39677d21.js", "./VListItem-b9e24cb0.css", "./VMenu-240a4406.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-04ae357c.js", "./VCard-103d8462.css", "./VSpacer-82874439.js", "./VSelect-4d69c543.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
                 props: !0
             }, {
                 path: "",
                 redirect: "/settings/providers",
                 name: "settingsredirect"
             }]
         }]
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ecb9e627.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/index-ecb9e627.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/layout-b0232ef9.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/layout-ff13c6fd.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     n as ee
-} from "./VBtn-61e39030.js";
+} from "./VBtn-629f5316.js";
 import {
     p as N,
     ak as E,
     al as te,
     am as U,
     an as Z,
     s as q,
@@ -13,15 +13,15 @@
     c as s,
     b as ae,
     r as se,
     aq as $,
     a as R,
     o as ue,
     ar as le
-} from "./index-ade73b84.js";
+} from "./index-a5bb9833.js";
 const M = Symbol.for("vuetify:layout"),
     D = Symbol.for("vuetify:layout-item"),
     K = 1e3,
     de = N({
         overlaps: {
             type: Array,
             default: () => []
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/logo-c9d5d6ab.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/logo-c9d5d6ab.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/m4a-45331b05.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/m4a-45331b05.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.ico` & `music-assistant-frontend-2.0.5/music_assistant_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.svg` & `music-assistant-frontend-2.0.5/music_assistant_frontend/favicon.svg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/index.html` & `music-assistant-frontend-2.0.5/music_assistant_frontend/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     <link rel="apple-touch-icon" href="apple-touch-icon.png" sizes="180x180">
     <link rel="mask-icon" href="favicon.svg" color="#FFFFFF">
     <link rel="manifest" href="manifest.webmanifest">
     <meta name="theme-color" content="#ffffff">
     <link rel="icon" href="favicon.ico" />
     <title>Music Assistant</title>
     <meta name="description" content="Music Assistant - Music library manager for Home Assistant">
-    <script type="module" crossorigin src="./assets/index-ade73b84.js"></script>
+    <script type="module" crossorigin src="./assets/index-a5bb9833.js"></script>
     <link rel="stylesheet" href="./assets/index-ecb9e627.css">
   <link rel="manifest" href="./manifest.webmanifest"><style>@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}</style></head>
   <body>
     <noscript>
       <strong
         >We're sorry but musicassistant-frontend doesn't work properly without
         JavaScript enabled. Please enable it to continue.</strong
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/manifest.webmanifest` & `music-assistant-frontend-2.0.5/music_assistant_frontend/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-192x192.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/pwa-192x192.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-512x512.png` & `music-assistant-frontend-2.0.5/music_assistant_frontend/pwa-512x512.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/sw.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/sw.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -26,244 +26,244 @@
     }
 }
 define(["./workbox-27b29e6f"], (function(s) {
     "use strict";
     self.addEventListener("message", (s => {
         s.data && "SKIP_WAITING" === s.data.type && self.skipWaiting()
     })), s.precacheAndRoute([{
-        url: "assets/AddProvider-a95ca786.js",
+        url: "assets/AddProvider-fa211913.js",
         revision: null
     }, {
-        url: "assets/AlbumDetails-55ac33a4.js",
+        url: "assets/AlbumDetails-ef8a3bee.js",
         revision: null
     }, {
-        url: "assets/Alert-4d78da02.js",
+        url: "assets/Alert-a5ce795e.js",
         revision: null
     }, {
         url: "assets/Alert-c80b13d7.css",
         revision: null
     }, {
-        url: "assets/ArtistDetails-7c7516d2.js",
+        url: "assets/ArtistDetails-cd5389ba.js",
         revision: null
     }, {
-        url: "assets/BrowseView-457188ac.js",
+        url: "assets/BrowseView-d5fa89c1.js",
         revision: null
     }, {
-        url: "assets/Button-15e2fa72.css",
+        url: "assets/Button-00834c6c.js",
         revision: null
     }, {
-        url: "assets/Button-4a781169.js",
+        url: "assets/Button-15e2fa72.css",
         revision: null
     }, {
-        url: "assets/Container-282a676b.js",
+        url: "assets/Container-4773c160.js",
         revision: null
     }, {
         url: "assets/Container-ed1c67df.css",
         revision: null
     }, {
         url: "assets/CoreConfigs-1c0e2549.css",
         revision: null
     }, {
-        url: "assets/CoreConfigs-69940384.js",
+        url: "assets/CoreConfigs-ec75d11a.js",
         revision: null
     }, {
-        url: "assets/Default-4e51f0b8.js",
+        url: "assets/Default-7879cbcb.js",
         revision: null
     }, {
         url: "assets/Default-8766b49d.css",
         revision: null
     }, {
         url: "assets/EditConfig-25e44c20.css",
         revision: null
     }, {
-        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js",
+        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js",
         revision: null
     }, {
-        url: "assets/EditCoreConfig-714d074a.js",
+        url: "assets/EditCoreConfig-37eaad58.js",
         revision: null
     }, {
-        url: "assets/EditPlayer-f0c55a15.js",
+        url: "assets/EditPlayer-33767eb3.js",
         revision: null
     }, {
-        url: "assets/EditProvider-a2553a06.js",
+        url: "assets/EditProvider-f88730fc.js",
         revision: null
     }, {
-        url: "assets/HomeView-af5707e7.js",
+        url: "assets/HomeView-95da878e.js",
         revision: null
     }, {
         url: "assets/HomeView-f559b858.css",
         revision: null
     }, {
-        url: "assets/index-ade73b84.js",
+        url: "assets/index-a5bb9833.js",
         revision: null
     }, {
         url: "assets/index-ecb9e627.css",
         revision: null
     }, {
         url: "assets/index.browser-7e542916.js",
         revision: null
     }, {
         url: "assets/InfoHeader-32cd2df9.css",
         revision: null
     }, {
-        url: "assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js",
+        url: "assets/InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js",
         revision: null
     }, {
         url: "assets/ItemsListing-7290acd0.css",
         revision: null
     }, {
-        url: "assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js",
+        url: "assets/ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js",
         revision: null
     }, {
-        url: "assets/layout-b0232ef9.js",
+        url: "assets/layout-ff13c6fd.js",
         revision: null
     }, {
-        url: "assets/LibraryAlbums-757b8aa2.js",
+        url: "assets/LibraryAlbums-55bc0ec5.js",
         revision: null
     }, {
-        url: "assets/LibraryArtists-225ce0c1.js",
+        url: "assets/LibraryArtists-0afc0ed9.js",
         revision: null
     }, {
-        url: "assets/LibraryPlaylists-4ffdc19f.js",
+        url: "assets/LibraryPlaylists-86c14bd9.js",
         revision: null
     }, {
-        url: "assets/LibraryRadios-a948d358.js",
+        url: "assets/LibraryRadios-3bd5ccff.js",
         revision: null
     }, {
-        url: "assets/LibraryTracks-5a540fa3.js",
+        url: "assets/LibraryTracks-07ab288b.js",
         revision: null
     }, {
-        url: "assets/ListviewItem-2bd74fad.js",
+        url: "assets/ListviewItem-707ff3c9.css",
         revision: null
     }, {
-        url: "assets/ListviewItem-732a7603.css",
+        url: "assets/ListviewItem-e2342ce8.js",
         revision: null
     }, {
         url: "assets/MediaItemThumb-24a77af5.css",
         revision: null
     }, {
-        url: "assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js",
+        url: "assets/MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js",
         revision: null
     }, {
         url: "assets/PanelviewItem-14a6b77a.css",
         revision: null
     }, {
-        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js",
+        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js",
         revision: null
     }, {
-        url: "assets/PlayerQueue-7ca94b07.js",
+        url: "assets/PlayerQueue-6206a6c6.js",
         revision: null
     }, {
-        url: "assets/Players-5c99fe5e.js",
+        url: "assets/Players-73f88aa0.js",
         revision: null
     }, {
-        url: "assets/PlaylistDetails-f8a1c191.js",
+        url: "assets/PlaylistDetails-ad67ce68.js",
         revision: null
     }, {
         url: "assets/Providers-0e527c0c.css",
         revision: null
     }, {
-        url: "assets/Providers-65d3d824.js",
+        url: "assets/Providers-0fb3a52e.js",
         revision: null
     }, {
-        url: "assets/RadioDetails-71dc877e.js",
+        url: "assets/RadioDetails-fb9a6d90.js",
         revision: null
     }, {
-        url: "assets/Search-f31ee239.js",
+        url: "assets/Search-1975e9f7.js",
         revision: null
     }, {
-        url: "assets/Settings-f159e60c.js",
+        url: "assets/Settings-05fc67af.js",
         revision: null
     }, {
-        url: "assets/TrackDetails-ca02e9b2.js",
+        url: "assets/TrackDetails-3d9e1c6f.js",
         revision: null
     }, {
-        url: "assets/VBadge-12aff0c7.js",
+        url: "assets/VBadge-9c063078.css",
         revision: null
     }, {
-        url: "assets/VBadge-9c063078.css",
+        url: "assets/VBadge-f7d58168.js",
         revision: null
     }, {
-        url: "assets/VBtn-61e39030.js",
+        url: "assets/VBtn-629f5316.js",
         revision: null
     }, {
         url: "assets/VBtn-76f512af.css",
         revision: null
     }, {
-        url: "assets/VCard-103d8462.css",
+        url: "assets/VCard-04ae357c.js",
         revision: null
     }, {
-        url: "assets/VCard-f3e11b51.js",
+        url: "assets/VCard-103d8462.css",
         revision: null
     }, {
         url: "assets/VDialog-28e4e64e.css",
         revision: null
     }, {
-        url: "assets/VDialog-93a2100b.js",
+        url: "assets/VDialog-667c0916.js",
         revision: null
     }, {
-        url: "assets/VDivider-adefbf87.js",
+        url: "assets/VDivider-bc1524a3.css",
         revision: null
     }, {
-        url: "assets/VDivider-bc1524a3.css",
+        url: "assets/VDivider-df9414f0.js",
         revision: null
     }, {
         url: "assets/VExpansionPanel-16e67e58.css",
         revision: null
     }, {
-        url: "assets/VExpansionPanel-75456689.js",
+        url: "assets/VExpansionPanel-1ca09b07.js",
         revision: null
     }, {
         url: "assets/VGrid-b9c72806.css",
         revision: null
     }, {
-        url: "assets/VListItem-b9e24cb0.css",
+        url: "assets/VListItem-39677d21.js",
         revision: null
     }, {
-        url: "assets/VListItem-f848c028.js",
+        url: "assets/VListItem-b9e24cb0.css",
         revision: null
     }, {
-        url: "assets/VMenu-b930657a.css",
+        url: "assets/VMenu-240a4406.js",
         revision: null
     }, {
-        url: "assets/VMenu-ccc026f2.js",
+        url: "assets/VMenu-b930657a.css",
         revision: null
     }, {
-        url: "assets/VRow-74a0e5a5.js",
+        url: "assets/VRow-7d86481a.js",
         revision: null
     }, {
         url: "assets/VSelect-45a454b3.css",
         revision: null
     }, {
-        url: "assets/VSelect-a66ffc02.js",
+        url: "assets/VSelect-4d69c543.js",
         revision: null
     }, {
-        url: "assets/VSpacer-159b0383.js",
+        url: "assets/VSpacer-82874439.js",
         revision: null
     }, {
-        url: "assets/VTabs-21d8affa.js",
+        url: "assets/VTabs-3cd3e980.css",
         revision: null
     }, {
-        url: "assets/VTabs-3cd3e980.css",
+        url: "assets/VTabs-f388999c.js",
         revision: null
     }, {
         url: "assets/VToolbar-222d6375.css",
         revision: null
     }, {
-        url: "assets/VToolbar-806969a3.js",
+        url: "assets/VToolbar-b79315e8.js",
         revision: null
     }, {
         url: "assets/vue-virtual-scroller-4d71315f.css",
         revision: null
     }, {
         url: "assets/workbox-window.prod.es5-a7b12eab.js",
         revision: null
     }, {
         url: "index.html",
-        revision: "fbf1a9e0c6d1935e8ef5886fdff83bbf"
+        revision: "ca22b0c8f3deb11f05e74b0e783dcfbb"
     }, {
         url: "favicon.svg",
         revision: "ecfda4076e793b6ffd619ed24e66c36d"
     }, {
         url: "favicon.ico",
         revision: "60d77c1713c2255be3f6de69c4de24d9"
     }, {
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend/workbox-27b29e6f.js` & `music-assistant-frontend-2.0.5/music_assistant_frontend/workbox-27b29e6f.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/PKG-INFO` & `music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.0.4
+Version: 2.0.5
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/SOURCES.txt` & `music-assistant-frontend-2.0.5/music_assistant_frontend.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,39 +16,39 @@
 music_assistant_frontend/sw.js
 music_assistant_frontend/workbox-27b29e6f.js
 music_assistant_frontend.egg-info/PKG-INFO
 music_assistant_frontend.egg-info/SOURCES.txt
 music_assistant_frontend.egg-info/dependency_links.txt
 music_assistant_frontend.egg-info/not-zip-safe
 music_assistant_frontend.egg-info/top_level.txt
-music_assistant_frontend/assets/AddProvider-a95ca786.js
-music_assistant_frontend/assets/AlbumDetails-55ac33a4.js
-music_assistant_frontend/assets/Alert-4d78da02.js
+music_assistant_frontend/assets/AddProvider-fa211913.js
+music_assistant_frontend/assets/AlbumDetails-ef8a3bee.js
+music_assistant_frontend/assets/Alert-a5ce795e.js
 music_assistant_frontend/assets/Alert-c80b13d7.css
-music_assistant_frontend/assets/ArtistDetails-7c7516d2.js
-music_assistant_frontend/assets/BrowseView-457188ac.js
+music_assistant_frontend/assets/ArtistDetails-cd5389ba.js
+music_assistant_frontend/assets/BrowseView-d5fa89c1.js
+music_assistant_frontend/assets/Button-00834c6c.js
 music_assistant_frontend/assets/Button-15e2fa72.css
-music_assistant_frontend/assets/Button-4a781169.js
-music_assistant_frontend/assets/Container-282a676b.js
+music_assistant_frontend/assets/Container-4773c160.js
 music_assistant_frontend/assets/Container-ed1c67df.css
 music_assistant_frontend/assets/CoreConfigs-1c0e2549.css
-music_assistant_frontend/assets/CoreConfigs-69940384.js
-music_assistant_frontend/assets/Default-4e51f0b8.js
+music_assistant_frontend/assets/CoreConfigs-ec75d11a.js
+music_assistant_frontend/assets/Default-7879cbcb.js
 music_assistant_frontend/assets/Default-8766b49d.css
 music_assistant_frontend/assets/EditConfig-25e44c20.css
-music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js
-music_assistant_frontend/assets/EditCoreConfig-714d074a.js
-music_assistant_frontend/assets/EditPlayer-f0c55a15.js
-music_assistant_frontend/assets/EditProvider-a2553a06.js
-music_assistant_frontend/assets/HomeView-af5707e7.js
+music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-8da5990b.js
+music_assistant_frontend/assets/EditCoreConfig-37eaad58.js
+music_assistant_frontend/assets/EditPlayer-33767eb3.js
+music_assistant_frontend/assets/EditProvider-f88730fc.js
+music_assistant_frontend/assets/HomeView-95da878e.js
 music_assistant_frontend/assets/HomeView-f559b858.css
 music_assistant_frontend/assets/InfoHeader-32cd2df9.css
-music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js
+music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-ffdc6f99.js
 music_assistant_frontend/assets/ItemsListing-7290acd0.css
-music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js
+music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-83c47556.js
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
@@ -83,72 +83,72 @@
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
-music_assistant_frontend/assets/LibraryAlbums-757b8aa2.js
-music_assistant_frontend/assets/LibraryArtists-225ce0c1.js
-music_assistant_frontend/assets/LibraryPlaylists-4ffdc19f.js
-music_assistant_frontend/assets/LibraryRadios-a948d358.js
-music_assistant_frontend/assets/LibraryTracks-5a540fa3.js
-music_assistant_frontend/assets/ListviewItem-2bd74fad.js
-music_assistant_frontend/assets/ListviewItem-732a7603.css
+music_assistant_frontend/assets/LibraryAlbums-55bc0ec5.js
+music_assistant_frontend/assets/LibraryArtists-0afc0ed9.js
+music_assistant_frontend/assets/LibraryPlaylists-86c14bd9.js
+music_assistant_frontend/assets/LibraryRadios-3bd5ccff.js
+music_assistant_frontend/assets/LibraryTracks-07ab288b.js
+music_assistant_frontend/assets/ListviewItem-707ff3c9.css
+music_assistant_frontend/assets/ListviewItem-e2342ce8.js
 music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
 music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
 music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
 music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
 music_assistant_frontend/assets/MediaItemThumb-24a77af5.css
-music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js
+music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-a35ce75a.js
 music_assistant_frontend/assets/PanelviewItem-14a6b77a.css
-music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js
-music_assistant_frontend/assets/PlayerQueue-7ca94b07.js
-music_assistant_frontend/assets/Players-5c99fe5e.js
-music_assistant_frontend/assets/PlaylistDetails-f8a1c191.js
+music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-d218249a.js
+music_assistant_frontend/assets/PlayerQueue-6206a6c6.js
+music_assistant_frontend/assets/Players-73f88aa0.js
+music_assistant_frontend/assets/PlaylistDetails-ad67ce68.js
 music_assistant_frontend/assets/Providers-0e527c0c.css
-music_assistant_frontend/assets/Providers-65d3d824.js
-music_assistant_frontend/assets/RadioDetails-71dc877e.js
-music_assistant_frontend/assets/Search-f31ee239.js
-music_assistant_frontend/assets/Settings-f159e60c.js
-music_assistant_frontend/assets/TrackDetails-ca02e9b2.js
-music_assistant_frontend/assets/VBadge-12aff0c7.js
+music_assistant_frontend/assets/Providers-0fb3a52e.js
+music_assistant_frontend/assets/RadioDetails-fb9a6d90.js
+music_assistant_frontend/assets/Search-1975e9f7.js
+music_assistant_frontend/assets/Settings-05fc67af.js
+music_assistant_frontend/assets/TrackDetails-3d9e1c6f.js
 music_assistant_frontend/assets/VBadge-9c063078.css
-music_assistant_frontend/assets/VBtn-61e39030.js
+music_assistant_frontend/assets/VBadge-f7d58168.js
+music_assistant_frontend/assets/VBtn-629f5316.js
 music_assistant_frontend/assets/VBtn-76f512af.css
+music_assistant_frontend/assets/VCard-04ae357c.js
 music_assistant_frontend/assets/VCard-103d8462.css
-music_assistant_frontend/assets/VCard-f3e11b51.js
 music_assistant_frontend/assets/VDialog-28e4e64e.css
-music_assistant_frontend/assets/VDialog-93a2100b.js
-music_assistant_frontend/assets/VDivider-adefbf87.js
+music_assistant_frontend/assets/VDialog-667c0916.js
 music_assistant_frontend/assets/VDivider-bc1524a3.css
+music_assistant_frontend/assets/VDivider-df9414f0.js
 music_assistant_frontend/assets/VExpansionPanel-16e67e58.css
-music_assistant_frontend/assets/VExpansionPanel-75456689.js
+music_assistant_frontend/assets/VExpansionPanel-1ca09b07.js
 music_assistant_frontend/assets/VGrid-b9c72806.css
+music_assistant_frontend/assets/VListItem-39677d21.js
 music_assistant_frontend/assets/VListItem-b9e24cb0.css
-music_assistant_frontend/assets/VListItem-f848c028.js
+music_assistant_frontend/assets/VMenu-240a4406.js
 music_assistant_frontend/assets/VMenu-b930657a.css
-music_assistant_frontend/assets/VMenu-ccc026f2.js
-music_assistant_frontend/assets/VRow-74a0e5a5.js
+music_assistant_frontend/assets/VRow-7d86481a.js
 music_assistant_frontend/assets/VSelect-45a454b3.css
-music_assistant_frontend/assets/VSelect-a66ffc02.js
-music_assistant_frontend/assets/VSpacer-159b0383.js
-music_assistant_frontend/assets/VTabs-21d8affa.js
+music_assistant_frontend/assets/VSelect-4d69c543.js
+music_assistant_frontend/assets/VSpacer-82874439.js
 music_assistant_frontend/assets/VTabs-3cd3e980.css
+music_assistant_frontend/assets/VTabs-f388999c.js
 music_assistant_frontend/assets/VToolbar-222d6375.css
-music_assistant_frontend/assets/VToolbar-806969a3.js
+music_assistant_frontend/assets/VToolbar-b79315e8.js
 music_assistant_frontend/assets/cover_dark-75402cd0.png
 music_assistant_frontend/assets/cover_light-b832ae9e.png
 music_assistant_frontend/assets/crossfade-ba51f69a.png
 music_assistant_frontend/assets/hires-438c7046.png
-music_assistant_frontend/assets/index-ade73b84.js
+music_assistant_frontend/assets/index-a5bb9833.js
 music_assistant_frontend/assets/index-ecb9e627.css
 music_assistant_frontend/assets/index.browser-7e542916.js
 music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
-music_assistant_frontend/assets/layout-b0232ef9.js
+music_assistant_frontend/assets/layout-ff13c6fd.js
 music_assistant_frontend/assets/logo-c9d5d6ab.png
 music_assistant_frontend/assets/m4a-45331b05.png
 music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
 music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot
 music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff
 music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf
 music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2
```

### Comparing `music-assistant-frontend-2.0.4/pyproject.toml` & `music-assistant-frontend-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "music-assistant-frontend"
-version = "2.0.4"
+version = "2.0.5"
 description = "The Music Assistant frontend"
 readme = "README.md"
 authors = [
     { name = "The Music Assistant Authors", email = "m.vanderveldt@outlook.com" },
 ]
 requires-python = ">=3.9.0"
```

