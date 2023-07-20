# Comparing `tmp/music-assistant-frontend-2.0.3.tar.gz` & `tmp/music-assistant-frontend-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-assistant-frontend-2.0.3.tar", last modified: Thu Jul 20 11:48:48 2023, max compression
+gzip compressed data, was "music-assistant-frontend-2.0.4.tar", last modified: Thu Jul 20 16:34:21 2023, max compression
```

## Comparing `music-assistant-frontend-2.0.3.tar` & `music-assistant-frontend-2.0.4.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:48:48.429052 music-assistant-frontend-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 11:47:36.000000 music-assistant-frontend-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 11:47:36.000000 music-assistant-frontend-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 11:48:48.429052 music-assistant-frontend-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-20 11:47:36.000000 music-assistant-frontend-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:48:48.409053 music-assistant-frontend-2.0.3/music_assistant_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/apple-touch-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:48:48.429052 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/AddProvider-32056ca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/AlbumDetails-343f22cb.js
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Alert-55091fd0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Alert-c80b13d7.css
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ArtistDetails-7bca6a8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/BrowseView-d63a1e11.js
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Button-15e2fa72.css
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Button-59559304.js
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Container-349a0ac0.js
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Container-ed1c67df.css
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/CoreConfigs-0b98268a.js
--rw-r--r--   0 runner    (1001) docker     (123)    56884 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Default-27a728f1.js
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Default-8766b49d.css
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditConfig-25e44c20.css
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditCoreConfig-d3e464b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditPlayer-19592b08.js
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditProvider-019f1e2b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/HomeView-6873693d.js
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/HomeView-f559b858.css
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/InfoHeader-32cd2df9.css
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ItemsListing-7290acd0.css
--rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryAlbums-ea4898eb.js
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryArtists-be1957cb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryPlaylists-a9b54924.js
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryRadios-996c89ba.js
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryTracks-d64430e5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ListviewItem-9fa6da34.css
--rw-r--r--   0 runner    (1001) docker     (123)    33397 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ListviewItem-b7a4258b.js
--rw-r--r--   0 runner    (1001) docker     (123)   160576 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
--rw-r--r--   0 runner    (1001) docker     (123)   347588 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   125116 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   143452 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css
--rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/PanelviewItem-14a6b77a.css
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/PlayerQueue-29876489.js
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Players-b1f01106.js
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/PlaylistDetails-09b11191.js
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Providers-0e527c0c.css
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Providers-a361876b.js
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/RadioDetails-6f742445.js
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Search-b8c39f87.js
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Settings-244fcb0f.js
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/TrackDetails-71587bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBadge-9c063078.css
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBadge-9fa94f29.js
--rw-r--r--   0 runner    (1001) docker     (123)    26417 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBtn-68784d55.js
--rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBtn-76f512af.css
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VCard-103d8462.css
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VCard-138864fc.js
--rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDialog-28e4e64e.css
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDialog-5f240a62.js
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDivider-336c24cd.js
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDivider-bc1524a3.css
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css
--rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VExpansionPanel-67038b00.js
--rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VGrid-b9c72806.css
--rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VListItem-230d1393.js
--rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VListItem-b9e24cb0.css
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VMenu-b930657a.css
--rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VMenu-bc0cce60.js
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VRow-e8f3e51e.js
--rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VSelect-04a129eb.js
--rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VSelect-45a454b3.css
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VSpacer-bdf2f653.js
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VTabs-13127e50.js
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VTabs-3cd3e980.css
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VToolbar-222d6375.css
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VToolbar-daf2b89f.js
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/cover_dark-75402cd0.png
--rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/cover_light-b832ae9e.png
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/crossfade-ba51f69a.png
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/hires-438c7046.png
--rw-r--r--   0 runner    (1001) docker     (123)   402027 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/index-e9211ef1.js
--rw-r--r--   0 runner    (1001) docker     (123)   662925 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/index-ecb9e627.css
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/index.browser-7e542916.js
--rw-r--r--   0 runner    (1001) docker     (123)    28226 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/layout-4499d5bc.js
--rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/logo-c9d5d6ab.png
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/m4a-45331b05.png
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)  1280212 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot
--rw-r--r--   0 runner    (1001) docker     (123)   576748 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff
--rw-r--r--   0 runner    (1001) docker     (123)  1279992 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   396732 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 11:48:36.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/pwa-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/pwa-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 11:48:33.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/robots.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-07-20 11:48:38.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-20 11:48:38.000000 music-assistant-frontend-2.0.3/music_assistant_frontend/workbox-27b29e6f.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:48:48.409053 music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 11:48:47.000000 music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-07-20 11:48:48.000000 music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:48:47.000000 music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:48:46.000000 music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 11:48:48.000000 music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 11:48:02.000000 music-assistant-frontend-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:48:48.429052 music-assistant-frontend-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.823826 music-assistant-frontend-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 16:32:47.000000 music-assistant-frontend-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 16:32:47.000000 music-assistant-frontend-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 16:34:21.823826 music-assistant-frontend-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-20 16:32:47.000000 music-assistant-frontend-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.795827 music-assistant-frontend-2.0.4/music_assistant_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/apple-touch-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.823826 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AddProvider-a95ca786.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AlbumDetails-55ac33a4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-4d78da02.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-c80b13d7.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ArtistDetails-7c7516d2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/BrowseView-457188ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Button-15e2fa72.css
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Button-4a781169.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-282a676b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-ed1c67df.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/CoreConfigs-1c0e2549.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/CoreConfigs-69940384.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56884 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-4e51f0b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-8766b49d.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig-25e44c20.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditCoreConfig-714d074a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditPlayer-f0c55a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditProvider-a2553a06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/HomeView-af5707e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/HomeView-f559b858.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader-32cd2df9.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing-7290acd0.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15740 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14684 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15752 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryAlbums-757b8aa2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryArtists-225ce0c1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryPlaylists-4ffdc19f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryRadios-a948d358.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryTracks-5a540fa3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33420 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-2bd74fad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-732a7603.css
+-rw-r--r--   0 runner    (1001) docker     (123)   160576 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   347588 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   125116 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   143452 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css
+-rw-r--r--   0 runner    (1001) docker     (123)    30167 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PanelviewItem-14a6b77a.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlayerQueue-7ca94b07.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Players-5c99fe5e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlaylistDetails-f8a1c191.js
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Providers-0e527c0c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Providers-65d3d824.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/RadioDetails-71dc877e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Search-f31ee239.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Settings-f159e60c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/TrackDetails-ca02e9b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-12aff0c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-9c063078.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26417 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-61e39030.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23463 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-76f512af.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-103d8462.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-f3e11b51.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20501 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-28e4e64e.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-93a2100b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-adefbf87.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-bc1524a3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15070 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-75456689.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22815 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VGrid-b9c72806.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-b9e24cb0.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16504 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-f848c028.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-b930657a.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-ccc026f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VRow-74a0e5a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-45a454b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24137 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-a66ffc02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSpacer-159b0383.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-21d8affa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-3cd3e980.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-222d6375.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-806969a3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_dark-75402cd0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11831 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_light-b832ae9e.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/crossfade-ba51f69a.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/hires-438c7046.png
+-rw-r--r--   0 runner    (1001) docker     (123)   402667 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ade73b84.js
+-rw-r--r--   0 runner    (1001) docker     (123)   662925 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ecb9e627.css
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index.browser-7e542916.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28226 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/layout-b0232ef9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/logo-c9d5d6ab.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/m4a-45331b05.png
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)  1280212 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   576748 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff
+-rw-r--r--   0 runner    (1001) docker     (123)  1279992 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   396732 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 16:34:06.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 16:34:03.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-20 16:34:09.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-07-20 16:34:09.000000 music-assistant-frontend-2.0.4/music_assistant_frontend/workbox-27b29e6f.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:34:21.795827 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:34:19.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 16:34:21.000000 music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-20 16:33:17.000000 music-assistant-frontend-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:34:21.827826 music-assistant-frontend-2.0.4/setup.cfg
```

### Comparing `music-assistant-frontend-2.0.3/LICENSE` & `music-assistant-frontend-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/PKG-INFO` & `music-assistant-frontend-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.0.3
+Version: 2.0.4
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.0.3/README.md` & `music-assistant-frontend-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/apple-touch-icon.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/AddProvider-32056ca3.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/AddProvider-a95ca786.js`

 * *Files 5% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as P
-} from "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
 import {
     b as T,
     V as _,
     c as $
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as A
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     j as I
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     c as O
-} from "./VMenu-bc0cce60.js";
-import "./VExpansionPanel-67038b00.js";
-import "./VDialog-5f240a62.js";
-import "./VListItem-230d1393.js";
-import "./VSpacer-bdf2f653.js";
-import "./VSelect-04a129eb.js";
+} from "./VMenu-ccc026f2.js";
+import "./VExpansionPanel-75456689.js";
+import "./VDialog-93a2100b.js";
+import "./VListItem-f848c028.js";
+import "./VSpacer-159b0383.js";
+import "./VSelect-a66ffc02.js";
 const U = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/AlbumDetails-343f22cb.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlaylistDetails-f8a1c191.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,164 +1,100 @@
 import {
-    _ as k,
+    _,
     f as y
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
 import {
-    _ as D
-} from "./InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js";
+    _ as k
+} from "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js";
 import {
-    l as B,
-    r as _,
-    w as E,
-    o as T,
-    O as m,
-    af as g,
-    b as L,
-    q as s,
-    y as v,
-    j as n,
-    v as c,
-    x as f,
-    F as z,
-    z as N,
-    A as I,
-    M as b,
-    ah as F,
-    L as h
-} from "./index-e9211ef1.js";
-import {
-    L as $,
-    a as w
-} from "./Container-349a0ac0.js";
+    C as b
+} from "./Container-282a676b.js";
 import {
-    a as P
-} from "./VCard-138864fc.js";
-import "./ListviewItem-b7a4258b.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VBtn-68784d55.js";
-import "./VListItem-230d1393.js";
-import "./VDialog-5f240a62.js";
-import "./VToolbar-daf2b89f.js";
-import "./VSelect-04a129eb.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
-import "./Alert-55091fd0.js";
-import "./VSpacer-bdf2f653.js";
-import "./VBadge-9fa94f29.js";
-import "./VRow-e8f3e51e.js"; /* empty css              */
-import "./layout-4499d5bc.js";
-const oe = B({
-    __name: "AlbumDetails",
+    l as h,
+    r as c,
+    w,
+    o as I,
+    O as l,
+    af as D,
+    b as C,
+    q as E,
+    y as g,
+    j as n,
+    x as T
+} from "./index-ade73b84.js";
+import "./ListviewItem-2bd74fad.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VBtn-61e39030.js";
+import "./VListItem-f848c028.js";
+import "./VDialog-93a2100b.js";
+import "./VCard-f3e11b51.js";
+import "./VToolbar-806969a3.js";
+import "./VSelect-a66ffc02.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+import "./Alert-4d78da02.js";
+import "./VSpacer-159b0383.js";
+import "./VBadge-12aff0c7.js";
+import "./VRow-74a0e5a5.js"; /* empty css              */
+import "./layout-b0232ef9.js";
+const W = h({
+    __name: "PlaylistDetails",
     props: {
         itemId: {},
-        provider: {},
-        forceProviderVersion: {}
+        provider: {}
     },
-    setup(A) {
-        const o = A,
-            l = _(!1),
-            t = _(),
-            u = async function() {
-                t.value = await m.getAlbum(o.itemId, o.provider)
+    setup(d) {
+        const i = d,
+            s = c(!1),
+            o = c(),
+            p = async function() {
+                o.value = await l.getPlaylist(i.itemId, i.provider)
             };
-        E(() => o.itemId, e => {
-            e && u()
+        w(() => i.itemId, t => {
+            t && p()
         }, {
             immediate: !0
-        }), T(() => {
-            const e = m.subscribe(g.MEDIA_ITEM_ADDED, a => {
-                var i;
-                const r = a.data;
-                ((i = t.value) == null ? void 0 : i.uri) == r.uri && (l.value = !0)
+        }), I(() => {
+            const t = l.subscribe(D.MEDIA_ITEM_ADDED, e => {
+                var r;
+                const a = e.data;
+                ((r = o.value) == null ? void 0 : r.uri) == a.uri && (s.value = !0)
             });
-            L(e)
+            C(t)
         });
-        const C = async function(e, a, r, i, d = !0) {
-            const p = await m.getAlbumTracks(o.itemId, o.provider);
-            return y(p, e, a, r, i, d)
-        }, V = async function(e, a, r, i, d = !0) {
-            const p = await m.getAlbumVersions(o.itemId, o.provider);
-            return y(p, e, a, r, i, d)
+        const f = async function(t, e, a, r, v = !0) {
+            const m = [];
+            return await l.getPlaylistTracks(i.itemId, i.provider, u => {
+                console.log("chunk", u.length), m.push(...u)
+            }), y(m, t, e, a, r, v)
         };
-        return (e, a) => (s(), v("section", null, [n(D, {
-            item: t.value,
-            "active-provider": e.provider
-        }, null, 8, ["item", "active-provider"]), n(k, {
-            itemtype: "albumtracks",
-            "parent-item": t.value,
-            "show-provider": !1,
-            "show-favorites-only-filter": !1,
-            "load-data": C,
-            "sort-keys": ["track_number", "sort_name", "duration"],
-            "update-available": l.value,
-            onRefreshClicked: a[0] || (a[0] = r => {
-                u(), l.value = !1
-            }),
-            title: e.$t("tracks"),
-            checksum: e.provider + e.itemId
-        }, null, 8, ["parent-item", "update-available", "title", "checksum"]), n(k, {
-            itemtype: "albumversions",
-            "parent-item": t.value,
-            "show-provider": !0,
-            "show-favorites-only-filter": !1,
-            "load-data": V,
-            "sort-keys": ["provider", "sort_name", "year"],
-            "update-available": l.value,
-            onRefreshClicked: a[1] || (a[1] = r => {
-                u(), l.value = !1
-            }),
-            title: e.$t("other_versions"),
-            "hide-on-empty": !0,
-            checksum: e.provider + e.itemId
-        }, null, 8, ["parent-item", "update-available", "title", "checksum"]), t.value && t.value.provider == "library" ? (s(), c(P, {
-            key: 0,
-            style: {
-                "margin-left": "20px",
-                "margin-right": "20px"
-            }
-        }, {
-            default: f(() => [(s(!0), v(z, null, N(I(F)(t.value), r => (s(), v("div", {
-                key: r.provider_instance
-            }, [
-                [r.provider_domain, r.provider_instance].includes(e.provider) ? b("", !0) : (s(), c($, {
-                    key: 0,
-                    onClick: i => e.$router.replace({
-                        name: "album",
-                        params: {
-                            itemId: r.item_id,
-                            provider: r.provider_instance
-                        }
+        return (t, e) => {
+            var a;
+            return E(), g("section", null, [n(k, {
+                item: o.value,
+                "active-provider": (a = o.value) == null ? void 0 : a.provider_mappings[0].provider_domain
+            }, null, 8, ["item", "active-provider"]), n(b, null, {
+                default: T(() => [n(_, {
+                    itemtype: "playlisttracks",
+                    "parent-item": o.value,
+                    "show-provider": !1,
+                    "show-library": !1,
+                    "show-favorites-only-filter": !1,
+                    "show-track-number": !1,
+                    "load-data": f,
+                    "sort-keys": ["position", "position DESC", "sort_name", "sort_artist", "sort_album"],
+                    "update-available": s.value,
+                    onRefreshClicked: e[0] || (e[0] = r => {
+                        p(), s.value = !1
                     }),
-                    subtitle: e.$t("check_item_on_provider", [t.value.name, I(m).providerManifests[r.provider_domain].name])
-                }, {
-                    prepend: f(() => [h("div", null, [n(w, {
-                        domain: r.provider_domain,
-                        size: 30
-                    }, null, 8, ["domain"])])]),
-                    _: 2
-                }, 1032, ["onClick", "subtitle"])), e.provider != "library" && t.value.provider == "library" ? (s(), c($, {
-                    key: 1,
-                    onClick: a[2] || (a[2] = i => e.$router.replace({
-                        name: "album",
-                        params: {
-                            itemId: t.value.item_id,
-                            provider: t.value.provider
-                        }
-                    })),
-                    subtitle: e.$t("check_item_in_library", [t.value.name])
-                }, {
-                    prepend: f(() => [h("div", null, [n(w, {
-                        domain: "library",
-                        size: 30
-                    })])]),
-                    _: 1
-                }, 8, ["subtitle"])) : b("", !0)
-            ]))), 128))]),
-            _: 1
-        })) : b("", !0)]))
+                    title: t.$t("playlist_tracks")
+                }, null, 8, ["parent-item", "update-available", "title"])]),
+                _: 1
+            })])
+        }
     }
 });
 export {
-    oe as
+    W as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Alert-55091fd0.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-4d78da02.js`

 * *Files 2% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as N
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     e as Y
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 const me = Y("v-alert-title"),
     ye = ["success", "info", "warning", "error"],
     fe = D({
         border: {
             type: [Boolean, String],
             validator: e => typeof e == "boolean" || ["top", "end", "bottom", "start"].includes(e)
         },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Alert-c80b13d7.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Alert-c80b13d7.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/BrowseView-d63a1e11.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/BrowseView-457188ac.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -12,36 +12,36 @@
     x as u,
     v as m,
     M as c,
     A as V,
     O as L,
     B as f,
     ae as q,
-    U as M
-} from "./index-e9211ef1.js";
+    S as M
+} from "./index-ade73b84.js";
 import {
     L as N,
     s as O
-} from "./ListviewItem-b7a4258b.js"; /* empty css                             */
+} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
 import {
     C as P
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     l as T,
     k as D
-} from "./VBtn-68784d55.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VListItem-230d1393.js";
-import "./VDialog-5f240a62.js";
-import "./VCard-138864fc.js";
-import "./VToolbar-daf2b89f.js";
-import "./VSelect-04a129eb.js"; /* empty css              */
-const S = _({
+} from "./VBtn-61e39030.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VListItem-f848c028.js";
+import "./VDialog-93a2100b.js";
+import "./VCard-f3e11b51.js";
+import "./VToolbar-806969a3.js";
+import "./VSelect-a66ffc02.js"; /* empty css              */
+const U = _({
     __name: "BrowseView",
     props: {
         path: {}
     },
     setup(d) {
         const t = d,
             {
@@ -115,10 +115,10 @@
                 }, 8, ["items"])]
             }),
             _: 1
         })]))
     }
 });
 export {
-    S as
+    U as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Button-59559304.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Button-4a781169.js`

 * *Files 6% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as v
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     l as d
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 const m = {
     props: {
         variant: {
             type: String,
             default: ""
         }
     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Container-349a0ac0.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-282a676b.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -9,36 +9,36 @@
     Y as k,
     y as p,
     j as u,
     k as $,
     F as V,
     M as I,
     l as L,
-    O as r,
     A as o,
     X as f,
+    O as r,
     p as P,
     g as b,
     u as B
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     b as T,
     V as w
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     l as A,
     V as _,
     a as H,
     d as D,
     i as F
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     a as S,
     V as N
-} from "./VListItem-230d1393.js"; /* empty css              */
+} from "./VListItem-f848c028.js"; /* empty css              */
 const h = (t, a) => {
         const e = t.__vccOpts || t;
         for (const [n, m] of a) e[n] = m;
         return e
     },
     O = {
         props: {
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Container-ed1c67df.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Container-ed1c67df.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Default-27a728f1.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-4e51f0b8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -40,16 +40,16 @@
     L as C,
     M as S,
     N as P,
     O as b,
     P as Nt,
     Q as ke,
     R as Lt,
-    S as be,
-    U as re,
+    S as re,
+    U as be,
     V as we,
     W as me,
     X as Y,
     Y as Ce,
     Z as ue,
     _ as Q,
     $ as Ze,
@@ -63,98 +63,98 @@
     a7 as Dt,
     a8 as Ht,
     a9 as Wt,
     aa as Fe,
     ab as At,
     ac as Ft,
     ad as Ot
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     u as Be,
     a as Ut,
     V as ce,
     b as fe,
     c as Qt
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     m as tt,
     a as _e,
     b as lt,
     c as at,
     d as Re,
     u as ot,
     e as Ve,
     f as it,
     g as st,
     h as Yt,
-    t as jt,
     i as se,
+    t as jt,
     V as D,
     j as nt,
     k as Gt,
     l as rt,
     n as Xt
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     m as Me,
     u as Ee,
     a as Kt,
     b as Zt,
     c as Jt
-} from "./layout-4499d5bc.js";
+} from "./layout-b0232ef9.js";
 import {
     V as el,
     a as tl,
     b as ut
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     B as F
-} from "./Button-59559304.js";
+} from "./Button-4a781169.js";
 import {
     L as Z,
     _ as ve,
     C as ll
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     V as al,
-    i as ol,
-    a as il,
     _ as ct,
+    a as ol,
+    i as il,
     b as sl,
     c as nl,
     g as Oe
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
 import {
     m as rl,
     V as $e,
     a as ul,
     b as cl
-} from "./VToolbar-daf2b89f.js";
+} from "./VToolbar-806969a3.js";
 import {
     V as dt,
     a as dl,
     b as vl,
     c as ml,
     d as pl
-} from "./VExpansionPanel-67038b00.js";
+} from "./VExpansionPanel-75456689.js";
 import {
     V as ye
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     V as fl,
     a as vt,
     b as yl
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as hl
-} from "./VBadge-9fa94f29.js";
+} from "./VBadge-12aff0c7.js";
 import {
     V as _l,
     a as gl
-} from "./VDialog-5f240a62.js"; /* empty css              */
+} from "./VDialog-93a2100b.js"; /* empty css              */
 function bl(a) {
     let {
         rootEl: t,
         isSticky: o,
         layoutItemStyles: s
     } = a;
     const l = A(!1),
@@ -1996,15 +1996,15 @@
                 }),
                 l = k(() => {
                     if (c.selectedPlayer) return c.selectedPlayer.group_childs
                 }),
                 e = k(() => {
                     if (s.value) return s.value.current_item
                 }),
-                n = k(() => ne.theme.current.value.dark ? ol : il),
+                n = k(() => ne.theme.current.value.dark ? il : sl),
                 d = function(r) {
                     Ae.push({
                         name: "track",
                         params: {
                             itemId: r.item_id,
                             provider: r.provider
                         }
@@ -2159,15 +2159,15 @@
                                 style: Y({
                                     paddingTop: "1vh",
                                     flex: i(T)({
                                         breakpoint: "bp3",
                                         condition: "lt"
                                     }) ? "1 1 auto" : "0 1 auto"
                                 })
-                            }, [C("div", Pa, [v(sl)]), C("div", Sa, [C("div", xa, [v(he, {
+                            }, [C("div", Pa, [v(ol)]), C("div", Sa, [C("div", xa, [v(he, {
                                 "visible-components": {
                                     repeat: {
                                         isVisible: i(T)("bp3")
                                     },
                                     shuffle: {
                                         isVisible: i(T)("bp3")
                                     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Default-8766b49d.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Default-8766b49d.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditConfig-25e44c20.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig-25e44c20.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -6,73 +6,73 @@
     f as K,
     c as A,
     al as ie,
     aI as ue,
     k as J,
     l as se,
     I as de,
-    aO as v,
-    aP as H,
     w as oe,
     q as o,
     y as E,
     v as b,
     x as n,
     F as Q,
     z as W,
     K as w,
     N as h,
     M as F,
     A as p,
-    L as V
-} from "./index-e9211ef1.js";
+    L as V,
+    aO as v,
+    aP as H
+} from "./index-ade73b84.js";
 import {
     a as ne,
     b as re,
     c as ve,
     d as me,
     V as pe
-} from "./VExpansionPanel-67038b00.js";
+} from "./VExpansionPanel-75456689.js";
 import {
     a as ce,
     i as le,
     I as be,
     L as Ve,
     j as ke,
     l as T
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     d as ge,
     e as he,
     m as fe,
     u as Ce,
     c as X,
     V as $e,
     f as Y
-} from "./VDialog-5f240a62.js";
+} from "./VDialog-93a2100b.js";
 import {
     f as Ee
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     a as we,
     c as Se,
     d as Ue
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as qe
-} from "./VSpacer-bdf2f653.js";
+} from "./VSpacer-159b0383.js";
 import {
     V as Ie
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     c as Pe,
     d as Z,
     V as D,
     b as Re
-} from "./VSelect-04a129eb.js";
+} from "./VSelect-a66ffc02.js";
 const Te = _({
         ...ce(),
         ...ge()
     }, "VForm"),
     Ae = ee()({
         name: "VForm",
         props: Te(),
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditCoreConfig-d3e464b0.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditCoreConfig-714d074a.js`

 * *Files 4% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as $
-} from "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
 import {
     n as B
 } from "./index.browser-7e542916.js";
 import {
     b as O,
     V as p,
     c as E
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as h
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     j as S
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     c as T
-} from "./VMenu-bc0cce60.js";
-import "./VExpansionPanel-67038b00.js";
-import "./VDialog-5f240a62.js";
-import "./VListItem-230d1393.js";
-import "./VSpacer-bdf2f653.js";
-import "./VSelect-04a129eb.js";
+} from "./VMenu-ccc026f2.js";
+import "./VExpansionPanel-75456689.js";
+import "./VDialog-93a2100b.js";
+import "./VListItem-f848c028.js";
+import "./VSpacer-159b0383.js";
+import "./VSelect-a66ffc02.js";
 const A = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditPlayer-19592b08.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditPlayer-f0c55a15.js`

 * *Files 3% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     V as N,
     _ as B
-} from "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
 import {
     b as I,
     V as m,
     c as S
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as g
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     V as T
-} from "./VSelect-04a129eb.js";
-import "./VExpansionPanel-67038b00.js";
-import "./VBtn-68784d55.js";
-import "./VDialog-5f240a62.js";
-import "./VListItem-230d1393.js";
-import "./VMenu-bc0cce60.js";
-import "./VSpacer-bdf2f653.js";
+} from "./VSelect-a66ffc02.js";
+import "./VExpansionPanel-75456689.js";
+import "./VBtn-61e39030.js";
+import "./VDialog-93a2100b.js";
+import "./VListItem-f848c028.js";
+import "./VMenu-ccc026f2.js";
+import "./VSpacer-159b0383.js";
 const P = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/EditProvider-019f1e2b.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/EditProvider-a2553a06.js`

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     V as I,
     _ as O
-} from "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js";
+} from "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js";
 import {
     n as P
 } from "./index.browser-7e542916.js";
 import {
     b as U,
     V as _,
     c as x
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as h
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     V as A
-} from "./VSelect-04a129eb.js";
+} from "./VSelect-a66ffc02.js";
 import {
     j as D
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     c as q
-} from "./VMenu-bc0cce60.js";
-import "./VExpansionPanel-67038b00.js";
-import "./VDialog-5f240a62.js";
-import "./VListItem-230d1393.js";
-import "./VSpacer-bdf2f653.js";
+} from "./VMenu-ccc026f2.js";
+import "./VExpansionPanel-75456689.js";
+import "./VDialog-93a2100b.js";
+import "./VListItem-f848c028.js";
+import "./VSpacer-159b0383.js";
 const z = {
         key: 0,
         style: {
             "margin-left": "-5px",
             "margin-right": "-5px"
         }
     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/HomeView-6873693d.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/HomeView-af5707e7.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,34 @@
 import {
     V as r,
     a as m
-} from "./VRow-e8f3e51e.js";
+} from "./VRow-74a0e5a5.js";
 import {
     a as c
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as p
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     l as d,
     V as u
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
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
-} from "./index-e9211ef1.js"; /* empty css              */
+} from "./index-ade73b84.js"; /* empty css              */
 const v = {
         style: {
             "margin-left": "10px",
             "margin-right": "10px",
             "margin-top": "10px",
             "margin-bottom": "10px"
         }
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/InfoHeader-32cd2df9.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader-32cd2df9.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,9 +1,9 @@
 import {
-    p as S,
+    p as U,
     g as E,
     j as a,
     l as G,
     r as A,
     e as Y,
     I as q,
     J,
@@ -19,68 +19,68 @@
     A as f,
     L as y,
     K as h,
     N as d,
     k as H,
     F as I,
     z as M,
-    ai as R,
+    ah as R,
     aa as z,
-    U as Q,
+    S as Q,
     aj as W,
     O as X
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     a as Z,
     L as ee
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     _ as N,
     V as te,
-    g as U
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
+    g as j
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
 import {
     g as ae,
     a as ie
-} from "./ListviewItem-b7a4258b.js";
+} from "./ListviewItem-2bd74fad.js";
 import {
     b as oe,
-    a as j
-} from "./VListItem-230d1393.js";
+    a as D
+} from "./VListItem-f848c028.js";
 import {
     b as re,
     V as g,
     a as B,
     c as le,
     d as ne
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     a as se,
     i as me,
     V as c,
     l as P,
     k as de
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     b as ue,
     V as pe
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     b as ye,
     c as fe
-} from "./layout-4499d5bc.js";
+} from "./layout-b0232ef9.js";
 import {
     V as ge,
     a as ce
-} from "./VDialog-5f240a62.js";
-const ve = S({
+} from "./VDialog-93a2100b.js";
+const ve = U({
         ...se(),
         ...ye()
     }, "VLayout"),
-    D = E()({
+    S = E()({
         name: "VLayout",
         props: ve(),
         setup(v, l) {
             let {
                 slots: u
             } = l;
             const {
@@ -153,15 +153,15 @@
         style: {
             position: "absolute",
             float: "right",
             right: "15px",
             top: "15px"
         }
     },
-    Ue = G({
+    je = G({
         __name: "InfoHeader",
         props: {
             item: {},
             activeProvider: {}
         },
         setup(v) {
             const l = v,
@@ -172,15 +172,15 @@
                 } = Y(),
                 $ = new URL("" + new URL("info_gradient-a4aefd1d.jpg", import.meta.url).href, self.location).href,
                 V = q(),
                 {
                     t: T
                 } = J();
             K(() => l.item, async e => {
-                e && (b.topBarTitle = e.name, k.value = U(l.item, z.FANART) || U(l.item, z.THUMB), b.topBarContextMenuItems = ae([e], e, T))
+                e && (b.topBarTitle = e.name, k.value = j(l.item, z.FANART) || j(l.item, z.THUMB), b.topBarContextMenuItems = ae([e], e, T))
             }, {
                 immediate: !0
             }), O(() => {
                 b.topBarContextMenuItems = []
             });
             const C = function(e) {
                     V.push({
@@ -229,28 +229,28 @@
                 })), a(oe, {
                     width: "100%",
                     height: "100%",
                     cover: "",
                     class: "background-image",
                     src: k.value,
                     gradient: e.$vuetify.theme.current.dark ? "to bottom, rgba(0,0,0,.90), rgba(0,0,0,.75)" : "to bottom, rgba(255,255,255,.90), rgba(255,255,255,.75)"
-                }, null, 8, ["src", "gradient"]), e.item ? (o(), s(D, {
+                }, null, 8, ["src", "gradient"]), e.item ? (o(), s(S, {
                     key: 1,
                     style: {
                         margin: "0",
                         position: "absolute",
                         top: "50%",
                         "-ms-transform": "translateY(-50%)",
                         transform: "translateY(-50%)",
                         "padding-left": "15px",
                         "align-items": "center",
                         "padding-right": "15px"
                     }
                 }, {
-                    default: t(() => [e.$vuetify.display.mobile ? n("", !0) : (o(), m("div", be, [e.item.media_type && (e.item.media_type == f(Q).ARTIST || "owner" in e.item) ? (o(), m("div", he, [a(j, {
+                    default: t(() => [e.$vuetify.display.mobile ? n("", !0) : (o(), m("div", be, [e.item.media_type && (e.item.media_type == f(Q).ARTIST || "owner" in e.item) ? (o(), m("div", he, [a(D, {
                         size: "192"
                     }, {
                         default: t(() => [a(N, {
                             item: e.item,
                             height: 230,
                             width: 230
                         }, null, 8, ["item"])]),
@@ -382,15 +382,15 @@
                                 density: "comfortable"
                             }, {
                                 default: t(() => [(o(!0), m(I, null, M(f(ie)([e.item]), i => (o(), s(ee, {
                                     key: i.label,
                                     title: e.$t(i.label, i.labelArgs),
                                     onClick: p => i.action ? i.action() : ""
                                 }, {
-                                    prepend: t(() => [a(j, {
+                                    prepend: t(() => [a(D, {
                                         style: {
                                             "padding-right": "10px"
                                         }
                                     }, {
                                         default: t(() => [a(c, {
                                             icon: i.icon
                                         }, null, 8, ["icon"])]),
@@ -436,15 +436,15 @@
                         small: "",
                         outlined: ""
                     }, {
                         default: t(() => [h(d(i), 1)]),
                         _: 2
                     }, 1024))), 128))])) : n("", !0)])]),
                     _: 1
-                })) : n("", !0), e.item ? (o(), s(D, {
+                })) : n("", !0), e.item ? (o(), s(S, {
                     key: 2,
                     style: {
                         "z-index": "800",
                         height: "100%",
                         "padding-left": "15px"
                     }
                 }, {
@@ -478,9 +478,9 @@
                     _: 1
                 })]),
                 _: 1
             }, 8, ["modelValue"])]))
         }
     });
 export {
-    Ue as _
+    je as _
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ItemsListing-7290acd0.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing-7290acd0.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,66 +1,69 @@
 import {
-    _ as he,
-    L as ke,
-    i as we,
-    s as Ce
-} from "./ListviewItem-b7a4258b.js"; /* empty css                             */
-import {
-    p as Ve,
-    m as Se,
-    as as _e,
-    g as $e,
-    f as Ie,
-    d as Me,
+    _ as ye,
+    L as he,
+    i as ke,
+    s as we
+} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
+import {
+    p as Ce,
+    m as Ve,
+    as as Se,
+    g as _e,
+    f as $e,
+    d as Ie,
     r as g,
     w as z,
     o as j,
     j as r,
-    k as A,
-    at as Ae,
-    au as Ne,
+    k as N,
+    at as Me,
+    au as Ae,
     q as m,
-    y as N,
+    y as I,
     Y as U,
     M as y,
     L as O,
     N as F,
-    n as ne,
-    a5 as Fe,
-    a6 as Le,
-    l as Pe,
-    O as Be,
-    I as Oe,
-    b as ze,
-    v as S,
+    n as le,
+    a5 as Ne,
+    a6 as Fe,
+    l as Le,
+    O as Pe,
+    I as Be,
+    b as Oe,
     x as d,
-    z as Q,
-    F as X,
+    B as b,
+    v as $,
+    F as Q,
+    z as X,
     A as Z,
     K,
-    B as b,
-    W as Ee,
+    W as ze,
     D as w
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
-    _ as Te
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
+    _ as Ee
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
 import {
-    C as x,
+    C as Te,
     L as De
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
+import {
+    A as x
+} from "./Alert-4d78da02.js";
 import {
-    A as ee
-} from "./Alert-55091fd0.js";
+    a as ee
+} from "./VCard-f3e11b51.js";
 import {
     V as Re
-} from "./VToolbar-daf2b89f.js";
+} from "./VToolbar-806969a3.js";
 import {
     V as qe
-} from "./VSpacer-bdf2f653.js";
+} from "./VSpacer-159b0383.js";
 import {
     o as Ke,
     p as He,
     c as Ue,
     q as je,
     r as Ge,
     s as We,
@@ -68,84 +71,81 @@
     g as Je,
     i as Qe,
     w as Xe,
     x as Ze,
     l as P,
     V as D,
     k as xe
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     V as et
-} from "./VBadge-9fa94f29.js";
+} from "./VBadge-12aff0c7.js";
 import {
     m as tt,
     a as at,
-    f as ot,
     c as te,
-    b as lt,
-    V as nt
-} from "./VMenu-bc0cce60.js";
-import {
-    a as ae
-} from "./VCard-138864fc.js";
+    f as ot,
+    V as lt,
+    b as nt
+} from "./VMenu-ccc026f2.js";
 import {
-    V as oe
-} from "./VDivider-336c24cd.js";
+    V as ae
+} from "./VDivider-adefbf87.js";
 import {
     V as it
-} from "./VSelect-04a129eb.js";
+} from "./VSelect-a66ffc02.js";
 import {
     V as st,
     a as rt
-} from "./VRow-e8f3e51e.js";
-const ut = Ve({
+} from "./VRow-74a0e5a5.js";
+const ut = Ce({
         multiLine: Boolean,
         timeout: {
             type: [Number, String],
             default: 5e3
         },
         vertical: Boolean,
         ...Ke({
             location: "bottom"
         }),
         ...He(),
         ...Ue(),
         ...je(),
-        ...Se(),
-        ..._e(tt({
+        ...Ve(),
+        ...Se(tt({
             transition: "v-snackbar-transition"
         }), ["persistent", "noClickAnimation", "scrim", "scrollStrategy"])
     }, "VSnackbar"),
-    ct = $e()({
+    ct = _e()({
         name: "VSnackbar",
         props: ut(),
         emits: {
             "update:modelValue": a => !0
         },
         setup(a, p) {
             let {
                 slots: t
             } = p;
-            const s = Ie(a, "modelValue"),
+            const s = $e(a, "modelValue"),
                 {
                     locationStyles: C
                 } = Ge(a),
                 {
                     positionClasses: v
                 } = We(a),
                 {
                     scopeId: n
                 } = at(),
                 {
-                    themeClasses: _
-                } = Me(a),
+                    themeClasses: S
+                } = Ie(a),
                 {
                     colorClasses: L,
                     colorStyles: V,
-                    variantClasses: $
+                    variantClasses: _
                 } = Ye(a),
                 {
                     roundedClasses: l
                 } = Je(a),
                 o = g();
             z(s, f), z(() => a.timeout, f), j(() => {
                 s.value && f()
@@ -161,27 +161,27 @@
             }
 
             function h() {
                 window.clearTimeout(k)
             }
             return Qe(() => {
                 const [c] = te.filterProps(a);
-                return r(te, A({
+                return r(te, N({
                     ref: o,
                     class: ["v-snackbar", {
                         "v-snackbar--active": s.value,
                         "v-snackbar--multi-line": a.multiLine && !a.vertical,
                         "v-snackbar--vertical": a.vertical
                     }, v.value, a.class],
                     style: a.style
                 }, c, {
                     modelValue: s.value,
-                    "onUpdate:modelValue": I => s.value = I,
-                    contentProps: A({
-                        class: ["v-snackbar__wrapper", _.value, L.value, l.value, $.value],
+                    "onUpdate:modelValue": M => s.value = M,
+                    contentProps: N({
+                        class: ["v-snackbar__wrapper", S.value, L.value, l.value, _.value],
                         style: [C.value, V.value],
                         onPointerenter: h,
                         onPointerleave: f
                     }, c.contentProps),
                     persistent: !0,
                     noClickAnimation: !0,
                     scrim: !1,
@@ -205,33 +205,33 @@
                         }, [t.actions()])]
                     })],
                     activator: t.activator
                 })
             }), ot({}, o)
         }
     }),
-    ie = (a, p) => {
+    ne = (a, p) => {
         const t = a.__vccOpts || a;
         for (const [s, C] of p) t[s] = C;
         return t
     },
     dt = {},
-    mt = a => (Fe("data-v-259be2b2"), a = a(), Le(), a),
+    mt = a => (Ne("data-v-259be2b2"), a = a(), Fe(), a),
     vt = {
         class: "container"
     },
     ft = mt(() => O("div", {
         class: "spinner"
     }, null, -1)),
     pt = [ft];
 
 function gt(a, p) {
-    return m(), N("div", vt, pt)
+    return m(), I("div", vt, pt)
 }
-const bt = ie(dt, [
+const bt = ne(dt, [
         ["render", gt],
         ["__scopeId", "data-v-259be2b2"],
         ["__file", "/home/oumoussa/side-projects/infinite/src/components/Spinner.vue"]
     ]),
     yt = a => ({
         loading() {
             a.value = "loading"
@@ -252,15 +252,15 @@
     },
     kt = (a, p) => {
         const t = a.getBoundingClientRect();
         if (!p) return t.top >= 0 && t.bottom <= window.innerHeight;
         const s = p.getBoundingClientRect();
         return t.top >= s.top && t.bottom <= s.bottom
     },
-    le = a => {
+    oe = a => {
         a.parentEl = document.querySelector(a.target) || null;
         let p = `0px 0px ${a.distance}px 0px`;
         a.top && (p = `${a.distance}px 0px 0px 0px`);
         const t = new IntersectionObserver(s => {
             s[0].isIntersecting && (a.firstload && a.emit(), a.firstload = !0)
         }, {
             root: a.parentEl,
@@ -306,43 +306,43 @@
         }) {
             const t = a;
             let s = null;
             const C = g(null),
                 v = g("ready"),
                 {
                     top: n,
-                    firstload: _,
+                    firstload: S,
                     target: L,
                     distance: V
                 } = t,
                 {
-                    identifier: $
-                } = Ae(t),
+                    identifier: _
+                } = Me(t),
                 l = {
                     infiniteLoading: C,
                     target: L,
                     top: n,
-                    firstload: _,
+                    firstload: S,
                     distance: V,
                     prevHeight: 0,
                     parentEl: null
                 };
             l.emit = ht(p, yt(v), l);
             const o = () => z(v, async f => {
                     const h = l.parentEl || document.documentElement;
-                    await ne(), f == "loaded" && n && (h.scrollTop = h.scrollHeight - l.prevHeight), f == "loaded" && kt(C.value, l.parentEl) && l.emit(), f == "complete" && s.disconnect()
+                    await le(), f == "loaded" && n && (h.scrollTop = h.scrollHeight - l.prevHeight), f == "loaded" && kt(C.value, l.parentEl) && l.emit(), f == "complete" && s.disconnect()
                 }),
-                k = () => z($, () => {
-                    v.value = "ready", s.disconnect(), s = le(l)
+                k = () => z(_, () => {
+                    v.value = "ready", s.disconnect(), s = oe(l)
                 });
             return j(() => {
-                s = le(l), o(), $ && k()
-            }), Ne(() => {
+                s = oe(l), o(), _ && k()
+            }), Ae(() => {
                 s.disconnect()
-            }), (f, h) => (m(), N("div", {
+            }), (f, h) => (m(), I("div", {
                 ref_key: "infiniteLoading",
                 ref: C
             }, [v.value == "loading" ? U(f.$slots, "spinner", {
                 key: 0
             }, () => [r(bt)], !0) : y("v-if", !0), v.value == "complete" ? U(f.$slots, "complete", {
                 key: 1
             }, () => {
@@ -351,73 +351,76 @@
             }, !0) : y("v-if", !0), v.value == "error" ? U(f.$slots, "error", {
                 key: 2,
                 retry: l.emit
             }, () => {
                 var c;
                 return [O("span", wt, [O("span", null, F(((c = a.slots) == null ? void 0 : c.error) || "Oops something went wrong!"), 1), O("button", {
                     class: "retry",
-                    onClick: h[0] || (h[0] = (...I) => l.emit && l.emit(...I))
+                    onClick: h[0] || (h[0] = (...M) => l.emit && l.emit(...M))
                 }, " retry ")])]
             }, !0) : y("v-if", !0)], 512))
         }
     },
-    Vt = ie(Ct, [
+    Vt = ne(Ct, [
         ["__scopeId", "data-v-9d82030b"],
         ["__file", "/home/oumoussa/side-projects/infinite/src/components/InfiniteLoading.vue"]
     ]);
 const St = {
         key: 0
     },
     _t = {
-        key: 2
+        key: 0
     },
     $t = {
-        key: 3
+        key: 2
     },
     It = {
+        key: 3
+    },
+    Mt = {
         style: {
             height: "30px",
             "margin-top": "20px"
         }
     },
-    Ht = function(a, p, t, s, C, v = !0) {
-        var V, $;
+    Ut = function(a, p, t, s, C, v = !0) {
+        var V, _;
         let n = [];
         if (C) {
             const l = C.toLowerCase();
-            for (const o of a)(o.name.toLowerCase().includes(l) || "artist" in o && ((V = o.artist) != null && V.name.toLowerCase().includes(l)) || "album" in o && (($ = o.album) != null && $.name.toLowerCase().includes(l)) || "artists" in o && o.artists && o.artists[0].name.toLowerCase().includes(l)) && n.push(o)
+            for (const o of a)(o.name.toLowerCase().includes(l) || "artist" in o && ((V = o.artist) != null && V.name.toLowerCase().includes(l)) || "album" in o && ((_ = o.album) != null && _.name.toLowerCase().includes(l)) || "artists" in o && o.artists && o.artists[0].name.toLowerCase().includes(l)) && n.push(o)
         } else n = a;
         s == "sort_name" && n.sort((l, o) => (l.sort_name || l.name).localeCompare(o.sort_name || o.name)), s == "sort_album" && n.sort((l, o) => {
             var k, f;
             return (f = l.album) == null ? void 0 : f.name.localeCompare((k = o.album) == null ? void 0 : k.name)
         }), s == "sort_artist" && n.sort((l, o) => l.artists[0].name.localeCompare(o.artists[0].name)), s == "track_number" && (n.sort((l, o) => (l.track_number || 0) - (o.track_number || 0)), n.sort((l, o) => (l.disc_number || 0) - (o.disc_number || 0))), s == "position" && n.sort((l, o) => (l.position || 0) - (o.position || 0)), s == "position DESC" && n.sort((l, o) => (o.position || 0) - (l.position || 0)), s == "year" && n.sort((l, o) => (l.year || 0) - (o.year || 0)), s == "timestamp_added DESC" && n.sort((l, o) => (o.timestamp_added || 0) - (l.timestamp_added || 0)), s == "duration" && n.sort((l, o) => (l.duration || 0) - (o.duration || 0)), s == "provider" && n.sort((l, o) => l.provider.localeCompare(o.provider)), v && (n = n.filter(l => l.favorite));
-        const _ = n.length,
+        const S = n.length,
             L = n.slice(p, p + t);
         return {
             items: L,
             count: L.length,
             limit: t,
             offset: p,
-            total: _
+            total: S
         }
     },
-    Ut = Pe({
+    jt = Le({
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
-                default: Object.keys(Be.providers).length > 1
+                default: Object.keys(Pe.providers).length > 1
             },
             showAlbum: {
                 type: Boolean,
                 default: !0
             },
             showMenu: {
                 type: Boolean,
@@ -452,38 +455,38 @@
         },
         emits: ["refreshClicked"],
         setup(a, {
             emit: p
         }) {
             const t = a,
                 s = 100,
-                C = Oe(),
+                C = Be(),
                 v = g("list"),
                 n = g(""),
-                _ = g("sort_name"),
+                S = g("sort_name"),
                 L = g(!1),
                 V = g(!1),
-                $ = g(!1),
+                _ = g(!1),
                 l = g(0),
                 o = g([]),
                 k = g(),
                 f = g(!1),
                 h = g(!1),
                 c = g([]),
-                I = g(!1),
-                se = g(!1),
+                M = g(!1),
+                ie = g(!1),
                 E = g(!1),
                 T = g(!0),
-                re = function() {
-                    V.value ? V.value = !1 : (V.value = !0, ne(() => {
+                se = function() {
+                    V.value ? V.value = !1 : (V.value = !0, le(() => {
                         var e;
                         (e = document.getElementById("searchInput")) == null || e.focus()
                     }))
                 },
-                ue = function(e) {
+                re = function(e) {
                     return w({
                         breakpoint: "bp1",
                         condition: "lt",
                         offset: b.sizeNavigationMenu
                     }) ? 2 : w({
                         breakpoint: "bp1",
                         condition: "gt",
@@ -534,367 +537,362 @@
                         offset: b.sizeNavigationMenu
                     }) ? 8 : w({
                         breakpoint: "bp10",
                         condition: "gt",
                         offset: b.sizeNavigationMenu
                     }) ? 9 : 0
                 },
-                ce = function() {
+                ue = function() {
                     v.value === "panel" ? v.value = "list" : v.value = "panel", localStorage.setItem(`viewMode.${t.itemtype}`, v.value)
                 },
-                de = function() {
+                ce = function() {
                     h.value = !h.value;
                     const e = h.value ? "true" : "false";
-                    localStorage.setItem(`favoriteFilter.${t.itemtype}`, e), M(!0)
+                    localStorage.setItem(`favoriteFilter.${t.itemtype}`, e), A(!0)
                 },
-                me = function() {
+                de = function() {
                     T.value = !T.value;
                     const e = T.value ? "true" : "false";
-                    localStorage.setItem(`albumArtistsFilter.${t.itemtype}`, e), M(!0)
+                    localStorage.setItem(`albumArtistsFilter.${t.itemtype}`, e), A(!0)
                 },
                 G = function(e) {
                     return c.value.includes(e)
                 },
                 W = function(e, u) {
                     if (u) c.value.includes(e) || c.value.push(e);
                     else
                         for (let i = 0; i < c.value.length; i++) c.value[i] === e && c.value.splice(i, 1);
                     b.blockGlobalPlayMenu = c.value.length > 0
                 },
-                ve = function() {
+                me = function() {
                     c.value = [], E.value = !1, b.blockGlobalPlayMenu = !1
                 },
                 H = function() {
-                    c.value.length > 0 ? I.value = !0 : E.value = !E.value
+                    c.value.length > 0 ? M.value = !0 : E.value = !E.value
                 },
-                fe = function(e) {
-                    M(!0)
+                ve = function(e) {
+                    A(!0)
                 },
                 q = function(e) {
-                    c.value = [e], I.value = !0
+                    c.value = [e], M.value = !0
                 },
-                pe = function() {
-                    M(!0), p("refreshClicked")
+                fe = function() {
+                    A(!0), p("refreshClicked")
                 },
                 Y = function(e) {
                     var u;
-                    if (!we(e)) {
+                    if (!ke(e)) {
                         q(e);
                         return
                     } ["artist", "album", "playlist"].includes(e.media_type) || !((u = b.selectedPlayer) != null && u.available) ? C.push({
                         name: e.media_type,
                         params: {
                             itemId: e.item_id,
                             provider: e.provider
                         }
                     }) : q(e)
                 },
-                ge = function(e, u) {
-                    e !== void 0 && (_.value = e), localStorage.setItem(`sortBy.${t.itemtype}`, _.value), M(!0)
+                pe = function(e, u) {
+                    e !== void 0 && (S.value = e), localStorage.setItem(`sortBy.${t.itemtype}`, S.value), A(!0)
                 },
-                be = function(e) {
+                ge = function(e) {
                     if (o.value.length == 0) {
                         e.loaded();
                         return
                     }
                     if (k.value !== void 0 && l.value >= k.value) {
                         e.loaded();
                         return
                     }
-                    l.value += s, M().then(() => {
+                    l.value += s, A().then(() => {
                         e.loaded()
                     })
                 },
-                ye = function() {
+                be = function() {
                     localStorage.setItem("globalsearch", n.value), C.push({
                         name: "search",
                         params: {
                             initSearch: n.value
                         }
                     })
                 };
             z(() => n.value, e => {
-                e && (V.value = !0), M(!0)
+                e && (V.value = !0), A(!0)
             }), z(() => t.updateAvailable, e => {
-                e && o.value.length == 0 && M(!0)
+                e && o.value.length == 0 && A(!0)
             }), z(() => t.checksum, e => {
-                e && M(!0)
+                e && A(!0)
             });
-            const M = async function(e = !1, u = s) {
-                e && (l.value = 0, se.value = !1), f.value = !0;
-                const i = await t.loadData(l.value, u, _.value, n.value || "", h.value, T.value);
+            const A = async function(e = !1, u = s) {
+                e && (l.value = 0, ie.value = !1), f.value = !0;
+                const i = await t.loadData(l.value, u, S.value, n.value || "", h.value, T.value);
                 l.value ? o.value.push(...i.items) : o.value = i.items, k.value = i.total, f.value = !1;
                 let B = `search.${t.itemtype}`;
                 t.parentItem && (B += t.parentItem.item_id), localStorage.setItem(B, n.value)
             };
             j(() => {
                 const e = localStorage.getItem(`viewMode.${t.itemtype}`);
                 e && e !== "null" ? v.value = e : t.itemtype == "artists" || t.itemtype == "albums" ? v.value = "panel" : v.value = "list";
                 const u = localStorage.getItem(`sortBy.${t.itemtype}`);
-                if (u && u !== "null" ? _.value = u : _.value = t.sortKeys[0], t.showFavoritesOnlyFilter !== !1) {
+                if (u && u !== "null" ? S.value = u : S.value = t.sortKeys[0], t.showFavoritesOnlyFilter !== !1) {
                     const R = localStorage.getItem(`favoriteFilter.${t.itemtype}`);
                     R && R == "true" && (h.value = !0)
                 }
                 if (t.showAlbumArtistsOnlyFilter !== !1) {
                     const R = localStorage.getItem(`albumArtistsFilter.${t.itemtype}`);
                     R && (T.value = R == "true")
                 }
                 let i = `search.${t.itemtype}`;
                 t.parentItem && (i += t.parentItem.item_id);
                 const B = localStorage.getItem(i);
-                B && B !== "null" && (console.log("savedSearch", B), n.value = B), M(!0)
+                B && B !== "null" && (console.log("savedSearch", B), n.value = B), A(!0)
             });
             const J = function(e) {
-                I.value || (e.key === "a" && (e.ctrlKey || e.metaKey) ? (e.preventDefault(), c.value = o.value) : !$.value && e.key == "Backspace" ? n.value = n.value.slice(0, -1) : !$.value && e.key.length == 1 && (n.value += e.key, V.value = !0))
+                M.value || (e.key === "a" && (e.ctrlKey || e.metaKey) ? (e.preventDefault(), c.value = o.value) : !_.value && e.key == "Backspace" ? n.value = n.value.slice(0, -1) : !_.value && e.key.length == 1 && (n.value += e.key, V.value = !0))
             };
-            return document.addEventListener("keydown", J), ze(() => {
+            return document.addEventListener("keydown", J), Oe(() => {
                 document.removeEventListener("keydown", J)
-            }), (e, u) => e.hideOnEmpty && o.value.length == 0 ? y("", !0) : (m(), S(x, {
-                key: 0
-            }, {
-                default: d(() => [r(he, {
-                    modelValue: I.value,
-                    "onUpdate:modelValue": u[0] || (u[0] = i => I.value = i),
-                    items: c.value,
-                    "parent-item": e.parentItem,
-                    onClear: ve,
-                    onDelete: fe
-                }, null, 8, ["modelValue", "items", "parent-item"]), r(ae, null, {
-                    default: d(() => [r(Re, {
-                        density: "compact",
-                        variant: "flat",
-                        color: "transparent"
-                    }, {
-                        title: d(() => [!e.$vuetify.display.mobile && e.title ? (m(), N("span", St, F(e.title), 1)) : y("", !0)]),
-                        default: d(() => [r(qe), r(P, A(t, {
-                            icon: E.value ? "mdi-checkbox-multiple-outline" : "mdi-checkbox-multiple-blank-outline",
-                            variant: "plain",
-                            onClick: H,
-                            title: e.$t("tooltip.select_items")
-                        }), null, 16, ["icon", "title"]), e.showFavoritesOnlyFilter !== !1 ? (m(), S(P, A({
-                            key: 0
-                        }, t, {
-                            icon: "",
-                            variant: "plain",
-                            onClick: de,
-                            title: e.$t("tooltip.filter_favorites")
-                        }), {
-                            default: d(() => [r(D, {
-                                icon: h.value ? "mdi-heart" : "mdi-heart-outline"
-                            }, null, 8, ["icon"])]),
-                            _: 1
-                        }, 16, ["title"])) : y("", !0), e.showAlbumArtistsOnlyFilter ? (m(), S(P, A({
-                            key: 1
-                        }, t, {
-                            icon: "",
-                            variant: "plain",
-                            onClick: me,
-                            title: e.$t("tooltip.album_artist_filter")
-                        }), {
-                            default: d(() => [r(D, {
-                                icon: T.value ? "mdi-account-music" : "mdi-account-music-outline"
-                            }, null, 8, ["icon"])]),
-                            _: 1
-                        }, 16, ["title"])) : y("", !0), r(P, A(t, {
-                            icon: "",
-                            variant: "plain",
-                            onClick: u[1] || (u[1] = i => pe()),
-                            title: e.updateAvailable ? e.$t("tooltip.refresh_new_content") : e.$t("tooltip.refresh")
-                        }), {
-                            default: d(() => [r(et, {
-                                "model-value": e.updateAvailable,
-                                color: "error",
-                                dot: ""
-                            }, {
-                                default: d(() => [r(D, {
-                                    icon: "mdi-refresh"
-                                })]),
-                                _: 1
-                            }, 8, ["model-value"])]),
-                            _: 1
-                        }, 16, ["title"]), e.sortKeys.length > 1 ? (m(), S(lt, {
-                            key: 2,
-                            modelValue: L.value,
-                            "onUpdate:modelValue": u[2] || (u[2] = i => L.value = i),
-                            location: "bottom end",
-                            "close-on-content-click": !0
+            }), (e, u) => e.hideOnEmpty && o.value.length == 0 ? y("", !0) : (m(), I("section", St, [r(ye, {
+                modelValue: M.value,
+                "onUpdate:modelValue": u[0] || (u[0] = i => M.value = i),
+                items: c.value,
+                "parent-item": e.parentItem,
+                onClear: me,
+                onDelete: ve
+            }, null, 8, ["modelValue", "items", "parent-item"]), r(ee, null, {
+                default: d(() => [r(Re, {
+                    density: "compact",
+                    variant: "flat",
+                    color: "transparent"
+                }, {
+                    title: d(() => [!e.$vuetify.display.mobile && e.title ? (m(), I("span", _t, F(e.title), 1)) : y("", !0)]),
+                    default: d(() => [r(qe), r(P, N(t, {
+                        icon: E.value ? "mdi-checkbox-multiple-outline" : "mdi-checkbox-multiple-blank-outline",
+                        variant: "plain",
+                        onClick: H,
+                        title: e.$t("tooltip.select_items")
+                    }), null, 16, ["icon", "title"]), e.showFavoritesOnlyFilter !== !1 ? (m(), $(P, N({
+                        key: 0
+                    }, t, {
+                        icon: "",
+                        variant: "plain",
+                        onClick: ce,
+                        title: e.$t("tooltip.filter_favorites")
+                    }), {
+                        default: d(() => [r(D, {
+                            icon: h.value ? "mdi-heart" : "mdi-heart-outline"
+                        }, null, 8, ["icon"])]),
+                        _: 1
+                    }, 16, ["title"])) : y("", !0), e.showAlbumArtistsOnlyFilter ? (m(), $(P, N({
+                        key: 1
+                    }, t, {
+                        icon: "",
+                        variant: "plain",
+                        onClick: de,
+                        title: e.$t("tooltip.album_artist_filter")
+                    }), {
+                        default: d(() => [r(D, {
+                            icon: T.value ? "mdi-account-music" : "mdi-account-music-outline"
+                        }, null, 8, ["icon"])]),
+                        _: 1
+                    }, 16, ["title"])) : y("", !0), r(P, N(t, {
+                        icon: "",
+                        variant: "plain",
+                        onClick: u[1] || (u[1] = i => fe()),
+                        title: e.updateAvailable ? e.$t("tooltip.refresh_new_content") : e.$t("tooltip.refresh")
+                    }), {
+                        default: d(() => [r(et, {
+                            "model-value": e.updateAvailable,
+                            color: "error",
+                            dot: ""
                         }, {
-                            activator: d(({
-                                props: i
-                            }) => [r(P, A({
-                                icon: ""
-                            }, i, {
-                                variant: "plain",
-                                title: e.$t("tooltip.sort_options")
-                            }), {
-                                default: d(() => [r(D, A(i, {
-                                    icon: "mdi-sort"
-                                }), null, 16)]),
-                                _: 2
-                            }, 1040, ["title"])]),
-                            default: d(() => [r(ae, null, {
-                                default: d(() => [r(nt, null, {
-                                    default: d(() => [(m(!0), N(X, null, Q(e.sortKeys, i => (m(), N("div", {
-                                        key: i
-                                    }, [r(De, {
-                                        onClick: B => ge(i)
-                                    }, {
-                                        title: d(() => [K(F(e.$t("sort." + i)), 1)]),
-                                        append: d(() => [_.value == i ? (m(), S(D, {
-                                            key: 0,
-                                            icon: "mdi-check"
-                                        })) : y("", !0)]),
-                                        _: 2
-                                    }, 1032, ["onClick"]), r(oe)]))), 128))]),
-                                    _: 1
-                                })]),
-                                _: 1
+                            default: d(() => [r(D, {
+                                icon: "mdi-refresh"
                             })]),
                             _: 1
-                        }, 8, ["modelValue"])) : y("", !0), r(P, A(t, {
-                            icon: "",
+                        }, 8, ["model-value"])]),
+                        _: 1
+                    }, 16, ["title"]), e.sortKeys.length > 1 ? (m(), $(nt, {
+                        key: 2,
+                        modelValue: L.value,
+                        "onUpdate:modelValue": u[2] || (u[2] = i => L.value = i),
+                        location: "bottom end",
+                        "close-on-content-click": !0
+                    }, {
+                        activator: d(({
+                            props: i
+                        }) => [r(P, N({
+                            icon: ""
+                        }, i, {
                             variant: "plain",
-                            onClick: u[3] || (u[3] = i => re()),
-                            title: e.$t("tooltip.search")
+                            title: e.$t("tooltip.sort_options")
                         }), {
-                            default: d(() => [r(D, {
-                                icon: "mdi-magnify"
+                            default: d(() => [r(D, N(i, {
+                                icon: "mdi-sort"
+                            }), null, 16)]),
+                            _: 2
+                        }, 1040, ["title"])]),
+                        default: d(() => [r(ee, null, {
+                            default: d(() => [r(lt, null, {
+                                default: d(() => [(m(!0), I(Q, null, X(e.sortKeys, i => (m(), I("div", {
+                                    key: i
+                                }, [r(De, {
+                                    onClick: B => pe(i)
+                                }, {
+                                    title: d(() => [K(F(e.$t("sort." + i)), 1)]),
+                                    append: d(() => [S.value == i ? (m(), $(D, {
+                                        key: 0,
+                                        icon: "mdi-check"
+                                    })) : y("", !0)]),
+                                    _: 2
+                                }, 1032, ["onClick"]), r(ae)]))), 128))]),
+                                _: 1
                             })]),
                             _: 1
-                        }, 16, ["title"]), r(P, A(t, {
-                            icon: v.value == "panel" ? "mdi-view-list" : "mdi-grid",
-                            variant: "plain",
-                            onClick: u[4] || (u[4] = i => ce()),
-                            title: e.$t("tooltip.toggle_view_mode")
-                        }), null, 16, ["icon", "title"])]),
+                        })]),
+                        _: 1
+                    }, 8, ["modelValue"])) : y("", !0), r(P, N(t, {
+                        icon: "",
+                        variant: "plain",
+                        onClick: u[3] || (u[3] = i => se()),
+                        title: e.$t("tooltip.search")
+                    }), {
+                        default: d(() => [r(D, {
+                            icon: "mdi-magnify"
+                        })]),
                         _: 1
-                    }), r(oe), V.value ? (m(), S(it, {
+                    }, 16, ["title"]), r(P, N(t, {
+                        icon: v.value == "panel" ? "mdi-view-list" : "mdi-grid",
+                        variant: "plain",
+                        onClick: u[4] || (u[4] = i => ue()),
+                        title: e.$t("tooltip.toggle_view_mode")
+                    }), null, 16, ["icon", "title"])]),
+                    _: 1
+                }), r(ae), V.value ? (m(), $(it, {
+                    key: 0,
+                    id: "searchInput",
+                    modelValue: n.value,
+                    "onUpdate:modelValue": u[5] || (u[5] = i => n.value = i),
+                    clearable: "",
+                    "prepend-inner-icon": "mdi-magnify",
+                    label: e.$t("search"),
+                    "hide-details": "",
+                    variant: "filled",
+                    style: {
+                        width: "auto",
+                        "margin-left": "15px",
+                        "margin-right": "15px",
+                        "margin-top": "10px"
+                    },
+                    onFocus: u[6] || (u[6] = i => _.value = !0),
+                    onBlur: u[7] || (u[7] = i => _.value = !1)
+                }, null, 8, ["modelValue", "label"])) : y("", !0), r(Te, null, {
+                    default: d(() => [f.value ? (m(), $(xe, {
                         key: 0,
-                        id: "searchInput",
-                        modelValue: n.value,
-                        "onUpdate:modelValue": u[5] || (u[5] = i => n.value = i),
-                        clearable: "",
-                        "prepend-inner-icon": "mdi-magnify",
-                        label: e.$t("search"),
-                        "hide-details": "",
-                        variant: "filled",
-                        style: {
-                            width: "auto",
-                            "margin-left": "15px",
-                            "margin-right": "15px",
-                            "margin-top": "10px"
-                        },
-                        onFocus: u[6] || (u[6] = i => $.value = !0),
-                        onBlur: u[7] || (u[7] = i => $.value = !1)
-                    }, null, 8, ["modelValue", "label"])) : y("", !0), r(x, null, {
-                        default: d(() => [f.value ? (m(), S(xe, {
-                            key: 0,
-                            indeterminate: ""
-                        })) : y("", !0), v.value == "panel" ? (m(), S(st, {
-                            key: 1
-                        }, {
-                            default: d(() => [(m(!0), N(X, null, Q(o.value, i => (m(), S(rt, {
-                                key: i.uri,
-                                class: Ee(`col-${ue(e.$vuetify.display.width)}`)
-                            }, {
-                                default: d(() => [r(Te, {
-                                    item: i,
-                                    "is-selected": G(i),
-                                    "show-checkboxes": E.value,
-                                    "show-track-number": e.showTrackNumber,
-                                    onSelect: W,
-                                    onMenu: q,
-                                    onClick: Y
-                                }, null, 8, ["item", "is-selected", "show-checkboxes", "show-track-number"])]),
-                                _: 2
-                            }, 1032, ["class"]))), 128))]),
-                            _: 1
-                        })) : y("", !0), v.value == "list" ? (m(), N("div", _t, [r(Z(Ce), {
-                            items: o.value,
-                            "item-size": 70,
-                            "key-field": "uri",
-                            "page-mode": ""
+                        indeterminate: ""
+                    })) : y("", !0), v.value == "panel" ? (m(), $(st, {
+                        key: 1
+                    }, {
+                        default: d(() => [(m(!0), I(Q, null, X(o.value, i => (m(), $(rt, {
+                            key: i.uri,
+                            class: ze(`col-${re(e.$vuetify.display.width)}`)
                         }, {
-                            default: d(({
-                                item: i
-                            }) => [(m(), S(ke, {
-                                key: i.uri,
+                            default: d(() => [r(Ee, {
                                 item: i,
-                                "show-track-number": e.showTrackNumber,
-                                "show-disc-number": e.showTrackNumber,
-                                "show-duration": e.showDuration,
-                                "show-favorite": e.showFavoritesOnlyFilter,
-                                "show-menu": e.showMenu,
-                                "show-provider": e.showProvider,
-                                "show-album": e.showAlbum,
-                                "show-checkboxes": E.value,
                                 "is-selected": G(i),
-                                "show-details": e.itemtype.includes("versions"),
-                                "parent-item": e.parentItem,
+                                "show-checkboxes": E.value,
+                                "show-track-number": e.showTrackNumber,
                                 onSelect: W,
                                 onMenu: q,
                                 onClick: Y
-                            }, null, 8, ["item", "show-track-number", "show-disc-number", "show-duration", "show-favorite", "show-menu", "show-provider", "show-album", "show-checkboxes", "is-selected", "show-details", "parent-item"]))]),
-                            _: 1
-                        }, 8, ["items"])])) : y("", !0), r(Z(Vt), {
-                            onInfinite: be
-                        }), !f.value && o.value.length == 0 ? (m(), N("div", $t, [!f.value && o.value.length == 0 && (n.value || h.value) ? (m(), S(ee, {
+                            }, null, 8, ["item", "is-selected", "show-checkboxes", "show-track-number"])]),
+                            _: 2
+                        }, 1032, ["class"]))), 128))]),
+                        _: 1
+                    })) : y("", !0), v.value == "list" ? (m(), I("div", $t, [r(Z(we), {
+                        items: o.value,
+                        "item-size": 70,
+                        "key-field": "uri",
+                        "page-mode": ""
+                    }, {
+                        default: d(({
+                            item: i
+                        }) => [(m(), $(he, {
+                            key: i.uri,
+                            item: i,
+                            "show-track-number": e.showTrackNumber,
+                            "show-disc-number": e.showTrackNumber,
+                            "show-duration": e.showDuration,
+                            "show-favorite": e.showFavoritesOnlyFilter,
+                            "show-menu": e.showMenu,
+                            "show-provider": e.showProvider,
+                            "show-album": e.showAlbum,
+                            "show-checkboxes": E.value,
+                            "is-selected": G(i),
+                            "show-details": e.itemtype.includes("versions"),
+                            "parent-item": e.parentItem,
+                            onSelect: W,
+                            onMenu: q,
+                            onClick: Y
+                        }, null, 8, ["item", "show-track-number", "show-disc-number", "show-duration", "show-favorite", "show-menu", "show-provider", "show-album", "show-checkboxes", "is-selected", "show-details", "parent-item"]))]),
+                        _: 1
+                    }, 8, ["items"])])) : y("", !0), r(Z(Vt), {
+                        onInfinite: ge
+                    }), !f.value && o.value.length == 0 ? (m(), I("div", It, [!f.value && o.value.length == 0 && (n.value || h.value) ? (m(), $(x, {
+                        key: 0,
+                        title: e.$t("no_content_filter")
+                    }, {
+                        default: d(() => [n.value ? (m(), $(P, {
                             key: 0,
-                            title: e.$t("no_content_filter")
-                        }, {
-                            default: d(() => [n.value ? (m(), S(P, {
-                                key: 0,
-                                style: {
-                                    "margin-top": "15px"
-                                },
-                                onClick: ye
-                            }, {
-                                default: d(() => [K(F(e.$t("try_global_search")), 1)]),
-                                _: 1
-                            })) : y("", !0)]),
-                            _: 1
-                        }, 8, ["title"])) : !f.value && o.value.length == 0 ? (m(), S(ee, {
-                            key: 1
+                            style: {
+                                "margin-top": "15px"
+                            },
+                            onClick: be
                         }, {
-                            default: d(() => [K(F(e.$t("no_content")), 1)]),
+                            default: d(() => [K(F(e.$t("try_global_search")), 1)]),
                             _: 1
-                        })) : y("", !0)])) : y("", !0), r(ct, {
-                            "model-value": c.value.length > 1,
-                            timeout: -1,
-                            style: {
-                                "margin-bottom": "120px"
-                            }
+                        })) : y("", !0)]),
+                        _: 1
+                    }, 8, ["title"])) : !f.value && o.value.length == 0 ? (m(), $(x, {
+                        key: 1
+                    }, {
+                        default: d(() => [K(F(e.$t("no_content")), 1)]),
+                        _: 1
+                    })) : y("", !0)])) : y("", !0), r(ct, {
+                        "model-value": c.value.length > 1,
+                        timeout: -1,
+                        style: {
+                            "margin-bottom": "120px"
+                        }
+                    }, {
+                        actions: d(() => [r(P, {
+                            color: "primary",
+                            variant: "text",
+                            onClick: u[8] || (u[8] = i => M.value = !0)
                         }, {
-                            actions: d(() => [r(P, {
-                                color: "primary",
-                                variant: "text",
-                                onClick: u[8] || (u[8] = i => I.value = !0)
-                            }, {
-                                default: d(() => [K(F(e.$t("actions")), 1)]),
-                                _: 1
-                            })]),
-                            default: d(() => [O("span", null, F(e.$t("items_selected", [c.value.length])), 1)]),
+                            default: d(() => [K(F(e.$t("actions")), 1)]),
                             _: 1
-                        }, 8, ["model-value"]), O("div", It, [!c.value.length && k.value ? (m(), N("span", {
-                            key: 0,
-                            style: {
-                                cursor: "pointer"
-                            },
-                            onClick: H
-                        }, F(e.$t("items_total", [k.value])), 1)) : c.value.length ? (m(), N("span", {
-                            key: 1,
-                            style: {
-                                cursor: "pointer"
-                            },
-                            onClick: H
-                        }, F(e.$t("items_selected", [c.value.length])), 1)) : y("", !0)])]),
+                        })]),
+                        default: d(() => [O("span", null, F(e.$t("items_selected", [c.value.length])), 1)]),
                         _: 1
-                    })]),
+                    }, 8, ["model-value"]), O("div", Mt, [!c.value.length && k.value ? (m(), I("span", {
+                        key: 0,
+                        style: {
+                            cursor: "pointer"
+                        },
+                        onClick: H
+                    }, F(e.$t("items_total", [k.value])), 1)) : c.value.length ? (m(), I("span", {
+                        key: 1,
+                        style: {
+                            cursor: "pointer"
+                        },
+                        onClick: H
+                    }, F(e.$t("items_selected", [c.value.length])), 1)) : y("", !0)])]),
                     _: 1
                 })]),
                 _: 1
-            }))
+            })]))
         }
     });
 export {
-    Ut as _, Ht as f
+    jt as _, Ut as f
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryAlbums-ea4898eb.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryArtists-225ce0c1.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,73 +1,71 @@
 import {
     l as d,
-    J as f,
+    J as v,
     r as i,
-    B as m,
-    O as r,
-    U as v,
-    b as n,
-    o as y,
+    B as n,
+    O as o,
+    S as y,
+    b as m,
+    o as E,
     af as s,
-    q as E,
-    v as D
-} from "./index-e9211ef1.js";
+    q as I,
+    v as A
+} from "./index-ade73b84.js";
 import {
-    _ as M
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js";
-import "./ListviewItem-b7a4258b.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VBtn-68784d55.js";
-import "./VListItem-230d1393.js";
-import "./Container-349a0ac0.js"; /* empty css              */
-import "./VDialog-5f240a62.js";
-import "./VCard-138864fc.js";
-import "./VToolbar-daf2b89f.js";
-import "./VSelect-04a129eb.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
-import "./Alert-55091fd0.js";
-import "./VSpacer-bdf2f653.js";
-import "./VBadge-9fa94f29.js";
-import "./VRow-e8f3e51e.js";
+    _ as D
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+import "./ListviewItem-2bd74fad.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VBtn-61e39030.js";
+import "./VListItem-f848c028.js";
+import "./Container-282a676b.js"; /* empty css              */
+import "./VDialog-93a2100b.js";
+import "./VCard-f3e11b51.js";
+import "./VToolbar-806969a3.js";
+import "./VSelect-a66ffc02.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+import "./Alert-4d78da02.js";
+import "./VSpacer-159b0383.js";
+import "./VBadge-12aff0c7.js";
+import "./VRow-74a0e5a5.js";
 const F = d({
-    __name: "LibraryAlbums",
-    setup(A) {
+    __name: "LibraryArtists",
+    setup(M) {
         const {
             t: p
-        } = f(), l = i([]), o = i(!1);
-        m.topBarContextMenuItems = [{
+        } = v(), l = i([]), r = i(!1), u = async function(t, a, e, c, _ = !0, f = !0) {
+            const b = _ || void 0;
+            return r.value = !1, await o.getLibraryArtists(b, c, a, t, e, f)
+        };
+        return n.topBarContextMenuItems = [{
             label: "sync_now",
-            labelArgs: [p("albums")],
+            labelArgs: [p("artists")],
             action: () => {
-                r.startSync([v.ALBUM])
+                o.startSync([y.ARTIST])
             },
             icon: "mdi-sync"
-        }], n(() => {
-            m.topBarContextMenuItems = []
-        }), y(() => {
-            const t = r.subscribe_multi([s.MEDIA_ITEM_ADDED, s.MEDIA_ITEM_UPDATED, s.MEDIA_ITEM_DELETED], a => {
+        }], m(() => {
+            n.topBarContextMenuItems = []
+        }), E(() => {
+            const t = o.subscribe_multi([s.MEDIA_ITEM_ADDED, s.MEDIA_ITEM_UPDATED, s.MEDIA_ITEM_DELETED], a => {
                 var e;
-                (e = a.object_id) != null && e.startsWith("library://artist") && (o.value = !0)
+                (e = a.object_id) != null && e.startsWith("library://artist") && (r.value = !0)
             });
-            n(t)
-        });
-        const u = async function(t, a, e, c, _ = !0) {
-            const b = _ || void 0;
-            return o.value = !1, await r.getLibraryAlbums(b, c, a, t, e)
-        };
-        return (t, a) => (E(), D(M, {
-            itemtype: "albums",
+            m(t)
+        }), (t, a) => (I(), A(D, {
+            itemtype: "artists",
             items: l.value,
             "show-provider": !1,
             "show-favorites-only-filter": !0,
             "load-data": u,
-            "sort-keys": ["sort_name", "timestamp_added DESC", "sort_artist", "year"],
-            "update-available": o.value
+            "show-album-artists-only-filter": !0,
+            "update-available": r.value
         }, null, 8, ["items", "update-available"]))
     }
 });
 export {
     F as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryPlaylists-a9b54924.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryPlaylists-4ffdc19f.js`

 * *Files 17% similar despite different names*

#### js-beautify {}

```diff
@@ -1,40 +1,40 @@
 import {
     l as y,
     J as v,
     r as l,
     B as r,
     O as o,
-    U as b,
+    S as b,
     ag as E,
     b as p,
     o as I,
     af as i,
     q as A,
     v as D
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as M
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js";
-import "./ListviewItem-b7a4258b.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VBtn-68784d55.js";
-import "./VListItem-230d1393.js";
-import "./Container-349a0ac0.js"; /* empty css              */
-import "./VDialog-5f240a62.js";
-import "./VCard-138864fc.js";
-import "./VToolbar-daf2b89f.js";
-import "./VSelect-04a129eb.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
-import "./Alert-55091fd0.js";
-import "./VSpacer-bdf2f653.js";
-import "./VBadge-9fa94f29.js";
-import "./VRow-e8f3e51e.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+import "./ListviewItem-2bd74fad.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VBtn-61e39030.js";
+import "./VListItem-f848c028.js";
+import "./Container-282a676b.js"; /* empty css              */
+import "./VDialog-93a2100b.js";
+import "./VCard-f3e11b51.js";
+import "./VToolbar-806969a3.js";
+import "./VSelect-a66ffc02.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+import "./Alert-4d78da02.js";
+import "./VSpacer-159b0383.js";
+import "./VBadge-12aff0c7.js";
+import "./VRow-74a0e5a5.js";
 const z = y({
     __name: "LibraryPlaylists",
     setup(T) {
         const {
             t: n
         } = v(), m = l([]), s = l(!1);
         r.topBarContextMenuItems = [{
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryRadios-996c89ba.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryRadios-a948d358.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,39 +1,39 @@
 import {
     l as v,
     J as y,
     r as n,
     B as m,
     O as o,
-    U as l,
+    S as l,
     b as p,
     o as I,
     af as i,
     q as D,
     v as E
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as A
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js";
-import "./ListviewItem-b7a4258b.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VBtn-68784d55.js";
-import "./VListItem-230d1393.js";
-import "./Container-349a0ac0.js"; /* empty css              */
-import "./VDialog-5f240a62.js";
-import "./VCard-138864fc.js";
-import "./VToolbar-daf2b89f.js";
-import "./VSelect-04a129eb.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
-import "./Alert-55091fd0.js";
-import "./VSpacer-bdf2f653.js";
-import "./VBadge-9fa94f29.js";
-import "./VRow-e8f3e51e.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+import "./ListviewItem-2bd74fad.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VBtn-61e39030.js";
+import "./VListItem-f848c028.js";
+import "./Container-282a676b.js"; /* empty css              */
+import "./VDialog-93a2100b.js";
+import "./VCard-f3e11b51.js";
+import "./VToolbar-806969a3.js";
+import "./VSelect-a66ffc02.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+import "./Alert-4d78da02.js";
+import "./VSpacer-159b0383.js";
+import "./VBadge-12aff0c7.js";
+import "./VRow-74a0e5a5.js";
 const F = v({
     __name: "LibraryRadios",
     setup(M) {
         const {
             t: s
         } = y(), u = n([]), r = n(!1);
         m.topBarContextMenuItems = [{
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/LibraryTracks-d64430e5.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/LibraryTracks-5a540fa3.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -1,39 +1,39 @@
 import {
     l as v,
     J as y,
     r as i,
     B as m,
     O as r,
-    U as l,
+    S as l,
     b as p,
     o as E,
     af as n,
     q as I,
     v as T
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as D
-} from "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js";
-import "./ListviewItem-b7a4258b.js";
-import "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VBtn-68784d55.js";
-import "./VListItem-230d1393.js";
-import "./Container-349a0ac0.js"; /* empty css              */
-import "./VDialog-5f240a62.js";
-import "./VCard-138864fc.js";
-import "./VToolbar-daf2b89f.js";
-import "./VSelect-04a129eb.js"; /* empty css                             */
-import "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
-import "./Alert-55091fd0.js";
-import "./VSpacer-bdf2f653.js";
-import "./VBadge-9fa94f29.js";
-import "./VRow-e8f3e51e.js";
+} from "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js";
+import "./ListviewItem-2bd74fad.js";
+import "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VBtn-61e39030.js";
+import "./VListItem-f848c028.js";
+import "./Container-282a676b.js"; /* empty css              */
+import "./VDialog-93a2100b.js";
+import "./VCard-f3e11b51.js";
+import "./VToolbar-806969a3.js";
+import "./VSelect-a66ffc02.js"; /* empty css                             */
+import "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
+import "./Alert-4d78da02.js";
+import "./VSpacer-159b0383.js";
+import "./VBadge-12aff0c7.js";
+import "./VRow-74a0e5a5.js";
 const z = v({
     __name: "LibraryTracks",
     setup(k) {
         const {
             t: s
         } = y(), c = i([]), o = i(!1);
         m.topBarContextMenuItems = [{
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ListviewItem-9fa6da34.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-732a7603.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.v-checkbox .v-selection-control{min-height:var(--v-input-control-height)}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}div.v-slide-group__next{position:absolute;right:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}div.v-slide-group__prev{position:absolute;left:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.content-spacing{display:flex;flex-flow:column;gap:10px}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.flicking-viewport{position:relative;overflow:hidden}.flicking-viewport.vertical{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex}.flicking-viewport.vertical>.flicking-camera{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}.flicking-viewport.flicking-hidden>.flicking-camera>*{visibility:hidden}.flicking-camera{width:100%;height:100%;display:-webkit-box;display:-ms-flexbox;display:flex;position:relative;-webkit-box-orient:horizontal;-webkit-box-direction:normal;-ms-flex-direction:row;flex-direction:row;z-index:1;will-change:transform}.flicking-camera>*{-ms-flex-negative:0;flex-shrink:0}.v-item-group{flex:0 1 auto;max-width:100%;position:relative;transition:.2s cubic-bezier(.4,0,.2,1)}.fullscreen-menu .v-overlay__content{left:0px;right:0px;top:0px;bottom:0px}.hiresicon[data-v-f28c82e3],.hiresicondark[data-v-f28c82e3]{margin-top:5px;margin-right:15px;margin-left:15px;filter:invert(100%)}
+@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.v-checkbox .v-selection-control{min-height:var(--v-input-control-height)}@font-face{font-family:Material Icons Outlined;font-style:normal;font-weight:400;src:url(./material-icons-outlined-35dca8a7.woff2) format("woff2")}.material-icons-outlined{font-family:Material Icons Outlined;font-weight:400;font-style:normal;font-size:24px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-webkit-font-feature-settings:"liga";-webkit-font-smoothing:antialiased}html{overflow:hidden}*{-webkit-user-drag:none;-khtml-user-drag:none;-moz-user-drag:none;-o-user-drag:none;user-drag:none;-webkit-touch-callout:none;-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}a{cursor:pointer}.v-btn--size-default{padding:0 8px}.vertical-btn{display:flex;flex-direction:column;align-items:center}.right{float:right}.left{float:left}.listitem-media-thumb{height:50px;width:50px;margin-right:10px}.v-slider.v-input--horizontal .v-input__control{min-height:5px}div.v-navigation-drawer__scrim{opacity:.8;background:grey}.v-card--variant-elevated{box-shadow:none;border-width:1px;border-style:solid;font-size:smaller}.line-clamp-2{white-space:pre-line;overflow:hidden;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.v-card-text{padding-right:0}.v-expansion-panel--active>.v-expansion-panel-title{min-height:48px}.col-2{width:50%;max-width:50%;flex-basis:50%}.col-3{width:33.3%;max-width:33.3%;flex-basis:33.3%}.col-4{width:25%;max-width:25%;flex-basis:25%}.col-5{width:20%;max-width:20%;flex-basis:20%}.col-6{width:16.6%;max-width:16.6%;flex-basis:16.6%}.col-7{width:14.2%;max-width:14.2%;flex-basis:14.2%}.col-8{width:12.5%;max-width:12.5%;flex-basis:12.5%}.col-9{width:11.1%;max-width:11.1%;flex-basis:11.1%}.line-clamp-1{white-space:nowrap;text-overflow:ellipsis;overflow:hidden}.line-clamp-2{white-space:pre-line;overflow:hidden;line-height:1.5em;height:3em;word-wrap:break-word;box-sizing:border-box;display:-webkit-box;-webkit-line-clamp:2}.small-icon{font-size:22px;height:22px;width:22px}.small-btn,.large-icon{font-size:40px;height:40px;width:40px}.large-btn{font-size:50px;height:50px;width:50px}div.v-slide-group__next{position:absolute;right:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}div.v-slide-group__prev{position:absolute;left:-5px;min-width:40px;height:30px;align-items:start;margin-top:-35px}.v-expansion-panel-title{border-radius:0}.v-input--horizontal .v-input__prepend{margin-inline-end:8px}.v-toolbar__content{height:100%!important}.content-spacing{display:flex;flex-flow:column;gap:10px}.padded-overlay .v-overlay__content{padding:50px}.v-overlay__scrim{opacity:65%}.v-expansion-panel-title{padding:10px}.flicking-camera{display:flex!important}.v-list-item-subtitle{font-size:.75rem;line-height:1rem;font-weight:400;margin-top:0;margin-bottom:0}.v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}.v-toolbar-title{font-size:1.25rem;line-height:1.75rem;font-weight:500}.v-list-item--nav .v-list-item-title{font-size:.875rem;line-height:1.25rem;font-weight:500}h1{font-size:1.5rem;line-height:2rem;font-weight:500}h2{font-size:1.25rem;line-height:1.75rem;font-weight:500}h3{font-size:1.125rem;line-height:1.5rem;font-weight:500}h4{font-size:1rem;line-height:1.25rem;font-weight:700}h5{font-size:.875rem;line-height:1.25rem;font-weight:500}h6{font-size:.75rem;line-height:1rem;font-weight:400}.mh1{margin-top:1.5rem;margin-bottom:1rem}.mh2{margin-top:1.5rem;margin-bottom:.75rem}.mh3{margin-top:1.5rem;margin-bottom:.5rem}.mh4{margin-top:1.25rem;margin-bottom:.5rem}.mh5{margin-top:1rem;margin-bottom:.25rem}.mh6{margin-top:1rem;margin-bottom:0}.flicking-viewport{position:relative;overflow:hidden}.flicking-viewport.vertical{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex}.flicking-viewport.vertical>.flicking-camera{display:-webkit-inline-box;display:-ms-inline-flexbox;display:inline-flex;-webkit-box-orient:vertical;-webkit-box-direction:normal;-ms-flex-direction:column;flex-direction:column}.flicking-viewport.flicking-hidden>.flicking-camera>*{visibility:hidden}.flicking-camera{width:100%;height:100%;display:-webkit-box;display:-ms-flexbox;display:flex;position:relative;-webkit-box-orient:horizontal;-webkit-box-direction:normal;-ms-flex-direction:row;flex-direction:row;z-index:1;will-change:transform}.flicking-camera>*{-ms-flex-negative:0;flex-shrink:0}.v-item-group{flex:0 1 auto;max-width:100%;position:relative;transition:.2s cubic-bezier(.4,0,.2,1)}.fullscreen-menu .v-overlay__content{left:0px;right:0px;top:0px;bottom:0px}.hiresicon[data-v-d473232c],.hiresicondark[data-v-d473232c]{margin-top:5px;margin-right:15px;margin-left:15px;filter:invert(100%)}
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/ListviewItem-b7a4258b.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/ListviewItem-2bd74fad.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -3,113 +3,113 @@
     a6 as qe,
     n as Me,
     q as u,
     v as V,
     aE as Xe,
     aF as Je,
     aG as Qe,
-    P as xe,
+    P as Ze,
     a9 as Le,
     Q as Oe,
     y as g,
     Y as ee,
     M as I,
     x as p,
     F as X,
     z as J,
     R as ke,
-    k as x,
-    aH as Ze,
+    k as Z,
+    aH as xe,
     X as et,
     W as me,
     j as y,
-    p as Be,
+    p as Re,
     as as tt,
     g as be,
     f as it,
     al as st,
     c as ge,
     aI as lt,
     m as rt,
     d as nt,
-    l as Re,
+    l as Be,
     J as Ee,
-    r as H,
+    r as K,
     w as ot,
-    O as w,
-    L as B,
+    L as R,
     N as S,
     A as b,
     K as F,
     B as te,
-    U as A,
+    O as w,
+    S as A,
     ag as Fe,
     aJ as at,
-    aK as W,
-    a4 as K,
-    aA as ie,
-    ai as Y,
+    aK as N,
+    a4 as j,
+    ah as Y,
     ae as ut,
     aj as dt,
-    a7 as se,
+    a7 as ie,
     D as ae,
-    S as ct
-} from "./index-e9211ef1.js";
+    U as ct,
+    aA as se
+} from "./index-ade73b84.js";
 import {
     _ as De,
     V as Ie,
     d as mt
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
 import {
     L as Q,
     a as fe,
     _ as ft
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     V as pt,
     b as Ve
-} from "./VToolbar-daf2b89f.js";
+} from "./VToolbar-806969a3.js";
 import {
     i as ht,
     a as yt,
     z as vt,
     d as bt,
     A as gt,
     B as _t,
     C as St,
     l as ne,
-    V as N
-} from "./VBtn-68784d55.js";
+    V as U
+} from "./VBtn-61e39030.js";
 import {
     V as wt
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     c as ue,
     a as kt
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     m as It,
     a as $e,
     b as Vt,
     V as $t
-} from "./VSelect-04a129eb.js";
+} from "./VSelect-a66ffc02.js";
 import {
     V as de
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     d as zt,
     a as ze,
     b as At
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     m as Tt,
     u as Ct,
     c as Ae,
     V as Pt
-} from "./VDialog-5f240a62.js";
+} from "./VDialog-93a2100b.js";
 
 function Mt() {
     var e = window.navigator.userAgent,
         t = e.indexOf("MSIE ");
     if (t > 0) return parseInt(e.substring(t + 5, e.indexOf(".", t)), 10);
     var i = e.indexOf("Trident/");
     if (i > 0) {
@@ -172,29 +172,29 @@
 const Lt = Xe();
 Ye("data-v-b329ee4c");
 const Ot = {
     class: "resize-observer",
     tabindex: "-1"
 };
 qe();
-const Bt = Lt((e, t, i, r, l, m) => (u(), V("div", Ot)));
-oe.render = Bt;
+const Rt = Lt((e, t, i, r, l, m) => (u(), V("div", Ot)));
+oe.render = Rt;
 oe.__scopeId = "data-v-b329ee4c";
 oe.__file = "src/components/ResizeObserver.vue";
 
 function re(e) {
     "@babel/helpers - typeof";
     return typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? re = function(t) {
         return typeof t
     } : re = function(t) {
         return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
     }, re(e)
 }
 
-function Rt(e, t) {
+function Bt(e, t) {
     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
 }
 
 function Te(e, t) {
     for (var i = 0; i < t.length; i++) {
         var r = t[i];
         r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
@@ -267,15 +267,15 @@
             if (!Ne(e[i], t[i])) return !1;
         return !0
     }
     return !1
 }
 var jt = function() {
     function e(t, i, r) {
-        Rt(this, e), this.el = t, this.observer = null, this.frozen = !1, this.createObserver(i, r)
+        Bt(this, e), this.el = t, this.observer = null, this.frozen = !1, this.createObserver(i, r)
     }
     return Et(e, [{
         key: "createObserver",
         value: function(i, r) {
             var l = this;
             if (this.observer && this.destroyObserver(), !this.frozen) {
                 if (this.options = Ht(i), this.callback = function(n, o) {
@@ -410,27 +410,27 @@
     },
     itemTag: {
         type: String,
         default: "div"
     }
 };
 
-function xt() {
+function Zt() {
     return this.items.length && ye(this.items[0]) !== "object"
 }
 var ve = !1;
 if (typeof window < "u") {
     ve = !1;
     try {
-        var Zt = Object.defineProperty({}, "passive", {
+        var xt = Object.defineProperty({}, "passive", {
             get: function() {
                 ve = !0
             }
         });
-        window.addEventListener("test", null, Zt)
+        window.addEventListener("test", null, xt)
     } catch {}
 }
 let ei = 0;
 var je = {
     name: "RecycleScroller",
     components: {
         ResizeObserver: oe
@@ -532,15 +532,15 @@
                     accumulator: m,
                     size: s
                 };
                 return this.$_computedMinItemSize = l, e
             }
             return []
         },
-        simpleArray: xt,
+        simpleArray: Zt,
         itemIndexByKey() {
             const {
                 keyField: e,
                 items: t
             } = this, i = {};
             for (let r = 0, l = t.length; r < l; r++) i[t[r][e]] = r;
             return i
@@ -636,16 +636,16 @@
                 s = this.typeField,
                 n = this.simpleArray ? null : this.keyField,
                 o = this.items,
                 f = o.length,
                 $ = this.sizes,
                 C = this.$_views,
                 M = this.$_unusedViews,
-                R = this.pool,
-                U = this.itemIndexByKey;
+                B = this.pool,
+                H = this.itemIndexByKey;
             let k, _, d, h, c;
             if (!f) k = _ = h = c = d = 0;
             else if (this.$_prerender) k = h = 0, _ = c = Math.min(this.prerender, o.length), d = null;
             else {
                 const v = this.getScroll();
                 if (t) {
                     let T = v.start - this.$_lastUpdateScrollPosition;
@@ -658,50 +658,50 @@
                 v.start -= L, v.end += L;
                 let z = 0;
                 if (this.$refs.before && (z = this.$refs.before.scrollHeight, v.start -= z), this.$refs.after) {
                     const T = this.$refs.after.scrollHeight;
                     v.end += T
                 }
                 if (i === null) {
-                    let T, G = 0,
+                    let T, W = 0,
                         Se = f - 1,
                         O = ~~(f / 2),
                         we;
-                    do we = O, T = $[O].accumulator, T < v.start ? G = O : O < f - 1 && $[O + 1].accumulator > v.start && (Se = O), O = ~~((G + Se) / 2); while (O !== we);
+                    do we = O, T = $[O].accumulator, T < v.start ? W = O : O < f - 1 && $[O + 1].accumulator > v.start && (Se = O), O = ~~((W + Se) / 2); while (O !== we);
                     for (O < 0 && (O = 0), k = O, d = $[f - 1].accumulator, _ = O; _ < f && $[_].accumulator < v.end; _++);
                     for (_ === -1 ? _ = o.length - 1 : (_++, _ > f && (_ = f)), h = k; h < f && z + $[h].accumulator < v.start; h++);
                     for (c = h; c < f && z + $[c].accumulator < v.end; c++);
                 } else {
                     k = ~~(v.start / i * r);
                     const T = k % r;
                     k -= T, _ = Math.ceil(v.end / i * r), h = Math.max(0, Math.floor((v.start - z) / i * r)), c = Math.floor((v.end - z) / i * r), k < 0 && (k = 0), _ > f && (_ = f), h < 0 && (h = 0), c > f && (c = f), d = Math.ceil(f / r) * i
                 }
             }
             _ - k > Yt.itemsLimit && this.itemsLimitError(), this.totalSize = d;
             let a;
             const P = k <= this.$_endIndex && _ >= this.$_startIndex;
             if (P)
-                for (let v = 0, L = R.length; v < L; v++) a = R[v], a.nr.used && (e && (a.nr.index = U[a.item[n]]), (a.nr.index == null || a.nr.index < k || a.nr.index >= _) && this.unuseView(a));
+                for (let v = 0, L = B.length; v < L; v++) a = B[v], a.nr.used && (e && (a.nr.index = H[a.item[n]]), (a.nr.index == null || a.nr.index < k || a.nr.index >= _) && this.unuseView(a));
             const _e = P ? null : new Map;
-            let D, E, Z;
+            let D, E, x;
             for (let v = k; v < _; v++) {
                 D = o[v];
                 const L = n ? D[n] : D;
                 if (L == null) throw new Error(`Key is ${L} on item (keyField is '${n}')`);
                 if (a = C.get(L), !i && !$[v].size) {
                     a && this.unuseView(a);
                     continue
                 }
                 E = D[s];
                 let z = M.get(E),
                     T = !1;
-                if (!a) P ? z && z.length ? a = z.pop() : a = this.addView(R, v, D, L, E) : (Z = _e.get(E) || 0, (!z || Z >= z.length) && (a = this.addView(R, v, D, L, E), this.unuseView(a, !0), z = M.get(E)), a = z[Z], _e.set(E, Z + 1)), C.delete(a.nr.key), a.nr.used = !0, a.nr.index = v, a.nr.key = L, a.nr.type = E, C.set(L, a), T = !0;
+                if (!a) P ? z && z.length ? a = z.pop() : a = this.addView(B, v, D, L, E) : (x = _e.get(E) || 0, (!z || x >= z.length) && (a = this.addView(B, v, D, L, E), this.unuseView(a, !0), z = M.get(E)), a = z[x], _e.set(E, x + 1)), C.delete(a.nr.key), a.nr.used = !0, a.nr.index = v, a.nr.key = L, a.nr.type = E, C.set(L, a), T = !0;
                 else if (!a.nr.used && (a.nr.used = !0, T = !0, z)) {
-                    const G = z.indexOf(a);
-                    G !== -1 && z.splice(G, 1)
+                    const W = z.indexOf(a);
+                    W !== -1 && z.splice(W, 1)
                 }
                 a.item = D, T && (v === o.length - 1 && this.$emit("scroll-end"), v === 0 && this.$emit("scroll-start")), i === null ? (a.position = $[v - 1].accumulator, a.offset = 0) : (a.position = Math.floor(v / r) * i, a.offset = v % r * l)
             }
             return this.$_startIndex = k, this.$_endIndex = _, this.emitUpdate && this.$emit("update", k, _, h, c), clearTimeout(this.$_sortTimer), this.$_sortTimer = setTimeout(this.sortViews, this.updateInterval + 300), {
                 continuous: P
             }
         },
@@ -785,15 +785,15 @@
     ii = {
         key: 1,
         ref: "after",
         class: "vue-recycle-scroller__slot"
     };
 
 function si(e, t, i, r, l, m) {
-    const s = xe("ResizeObserver"),
+    const s = Ze("ResizeObserver"),
         n = Le("observe-visibility");
     return Oe((u(), g("div", {
         class: me(["vue-recycle-scroller", {
             ready: l.ready,
             "page-mode": i.pageMode,
             [`direction-${e.direction}`]: !0
         }]),
@@ -801,25 +801,25 @@
     }, [e.$slots.before ? (u(), g("div", ti, [ee(e.$slots, "before")], 512)) : I("v-if", !0), (u(), V(ke(i.listTag), {
         ref: "wrapper",
         style: et({
             [e.direction === "vertical" ? "minHeight" : "minWidth"]: l.totalSize + "px"
         }),
         class: me(["vue-recycle-scroller__item-wrapper", i.listClass])
     }, {
-        default: p(() => [(u(!0), g(X, null, J(l.pool, o => (u(), V(ke(i.itemTag), x({
+        default: p(() => [(u(!0), g(X, null, J(l.pool, o => (u(), V(ke(i.itemTag), Z({
             key: o.nr.id,
             style: l.ready ? {
                 transform: `translate${e.direction==="vertical"?"Y":"X"}(${o.position}px) translate${e.direction==="vertical"?"X":"Y"}(${o.offset}px)`,
                 width: i.gridItems ? `${e.direction==="vertical"&&i.itemSecondarySize||i.itemSize}px` : void 0,
                 height: i.gridItems ? `${e.direction==="horizontal"&&i.itemSecondarySize||i.itemSize}px` : void 0
             } : null,
             class: ["vue-recycle-scroller__item-view", [i.itemClass, {
                 hover: !i.skipHover && l.hoverKey === o.nr.key
             }]]
-        }, Ze(i.skipHover ? {} : {
+        }, xe(i.skipHover ? {} : {
             mouseenter: () => {
                 l.hoverKey = o.nr.key
             },
             mouseleave: () => {
                 l.hoverKey = null
             }
         })), {
@@ -835,15 +835,15 @@
         onNotify: m.handleResize
     }, null, 8, ["onNotify"])], 34)), [
         [n, m.handleVisibilityChange]
     ])
 }
 je.render = si;
 je.__file = "src/components/RecycleScroller.vue";
-const li = Be({
+const li = Re({
         ...Tt(),
         ...tt(It(), ["inline"])
     }, "VCheckbox"),
     ri = be()({
         name: "VCheckbox",
         inheritAttrs: !1,
         props: li(),
@@ -861,16 +861,16 @@
                     isFocused: m,
                     focus: s,
                     blur: n
                 } = Ct(e),
                 o = st(),
                 f = ge(() => e.id || `checkbox-${o}`);
             return ht(() => {
-                const [$, C] = lt(i), [M, R] = Ae.filterProps(e), [U, k] = $e.filterProps(e);
-                return y(Ae, x({
+                const [$, C] = lt(i), [M, B] = Ae.filterProps(e), [H, k] = $e.filterProps(e);
+                return y(Ae, Z({
                     class: ["v-checkbox", e.class]
                 }, $, M, {
                     modelValue: l.value,
                     "onUpdate:modelValue": _ => l.value = _,
                     id: f.value,
                     focused: m.value,
                     style: e.style
@@ -879,15 +879,15 @@
                     default: _ => {
                         let {
                             id: d,
                             messagesId: h,
                             isDisabled: c,
                             isReadonly: a
                         } = _;
-                        return y($e, x(U, {
+                        return y($e, Z(H, {
                             id: d.value,
                             "aria-describedby": h.value,
                             disabled: c.value,
                             readonly: a.value
                         }, C, {
                             modelValue: l.value,
                             "onUpdate:modelValue": P => l.value = P,
@@ -896,15 +896,15 @@
                         }), r)
                     }
                 })
             }), {}
         }
     });
 const Ge = Symbol.for("vuetify:v-item-group"),
-    ni = Be({
+    ni = Re({
         ...yt(),
         ...vt({
             selectedClass: "v-item--selected"
         }),
         ...bt(),
         ...rt()
     }, "VItemGroup"),
@@ -980,43 +980,43 @@
     },
     ui = {
         class: "media-thumb"
     },
     di = {
         key: 0
     },
-    j = function(e) {
+    G = function(e) {
         var t;
         for (const i of e.provider_mappings)
             if (i.available && ((t = w.providers[i.provider_instance]) != null && t.available)) return !0;
         return !1
     },
     ci = function(e) {
         var t;
         for (const i of e.provider_mappings)
             if ((t = w.providers[i.provider_instance]) != null && t.supported_features.includes(Fe.SIMILAR_TRACKS)) return !0;
         return !1
     },
     mi = function(e, t) {
         const i = [];
-        if (e.length == 0 || !j(e[0])) return i;
-        let r = W.PLAY,
-            l = W.NEXT;
-        return (e.length > 10 || [A.ALBUM, A.PLAYLIST].includes(e[0].media_type)) && (r = W.REPLACE, l = W.REPLACE_NEXT), e.length == 1 && t && t.media_type == A.PLAYLIST && i.push({
+        if (e.length == 0 || !G(e[0])) return i;
+        let r = N.PLAY,
+            l = N.NEXT;
+        return (e.length > 10 || [A.ALBUM, A.PLAYLIST].includes(e[0].media_type)) && (r = N.REPLACE, l = N.REPLACE_NEXT), e.length == 1 && t && t.media_type == A.PLAYLIST && i.push({
             label: "play_playlist_from",
             action: () => {
-                w.playPlaylistFromIndex(t, e[0].position || 0)
+                w.playMedia(t, N.REPLACE, !1, e[0].item_id)
             },
             icon: "mdi-play-circle-outline",
             labelArgs: [],
             actionStr: "play"
         }), e.length == 1 && t && t.media_type == A.ALBUM && i.push({
             label: "play_album_from",
             action: () => {
-                w.playAlbumFromItem(t, e[0])
+                w.playMedia(t, N.REPLACE, !1, e[0].item_id)
             },
             icon: "mdi-play-circle-outline",
             labelArgs: [],
             actionStr: "play"
         }), i.push({
             label: "play_now",
             action: () => {
@@ -1040,90 +1040,90 @@
             },
             icon: "mdi-skip-next-circle-outline",
             labelArgs: [],
             actionStr: "play"
         }), i.push({
             label: "add_queue",
             action: () => {
-                w.playMedia(e, W.ADD)
+                w.playMedia(e, N.ADD)
             },
             icon: "mdi-playlist-plus",
             labelArgs: [],
             actionStr: "play"
         }), i
     },
     We = function(e, t, i) {
         const r = [];
         if (e.length == 0) return r;
-        if (e.length === 1 && e[0] !== t && j(e[0]) && r.push({
+        if (e.length === 1 && e[0] !== t && G(e[0]) && r.push({
                 label: "show_info",
                 labelArgs: [],
                 action: () => {
                     var l;
-                    K.push({
+                    j.push({
                         name: e[0].media_type,
                         params: {
                             itemId: e[0].item_id,
                             provider: e[0].provider
                         },
                         query: {
                             album: "album" in e[0] ? (l = e[0].album) == null ? void 0 : l.uri : ""
                         }
                     })
                 },
                 icon: "mdi-information-outline"
-            }), e.length === 1 && j(e[0]) && "artists" in e[0] && e[0].artists.length === 1)
+            }), e.length === 1 && G(e[0]) && "artists" in e[0] && e[0].artists.length === 1)
             for (const l of e[0].artists) r.push({
                 label: "goto_artist",
                 labelArgs: [l.name],
                 action: () => {
-                    K.push({
+                    j.push({
                         name: "artist",
                         params: {
                             itemId: l.item_id,
                             provider: l.provider
                         }
                     })
                 },
                 icon: "mdi-account-music"
             });
-        if (e.length === 1 && j(e[0]) && "album" in e[0] && e[0].album && r.push({
+        if (e.length === 1 && G(e[0]) && "album" in e[0] && e[0].album && r.push({
                 label: "goto_album",
                 labelArgs: [e[0].album.name],
                 action: () => {
-                    K.push({
+                    j.push({
                         name: "album",
                         params: {
                             itemId: e[0].album.item_id,
                             provider: e[0].album.provider
                         }
                     })
                 },
                 icon: "mdi-album"
-            }), e.length === 1 && (e[0] == t || !j(e[0])) && r.push({
+            }), e.length === 1 && (e[0] == t || !G(e[0])) && r.push({
                 label: "refresh_item",
                 labelArgs: [],
                 action: async () => {
-                    await w.refreshItem(e[0]), K.go(0)
+                    await w.refreshItem(e[0]), j.go(0)
                 },
                 icon: "mdi-refresh"
-            }), e[0].provider != "library" && j(e[0]) && r.push({
+            }), e[0].provider != "library" && G(e[0]) && r.push({
                 label: "add_library",
                 labelArgs: [],
                 action: () => {
                     for (const l of e) w.addItemToLibrary(l)
                 },
                 icon: "mdi-bookshelf"
             }), e[0].provider == "library" && r.push({
                 label: "remove_library",
                 labelArgs: [],
                 action: () => {
                     if (confirm(i("confirm_library_remove"))) {
                         for (const l of e) w.removeItemFromLibrary(l.media_type, l.item_id);
-                        e[0].item_id == (t == null ? void 0 : t.item_id) ? K.go(-1) : K.go(0)
+                        e[0].item_id == (t == null ? void 0 : t.item_id) ? j.go(-1) : j.go(0)
                     }
                 },
                 icon: "mdi-bookshelf"
             }), e[0].favorite || r.push({
                 label: "favorites_add",
                 labelArgs: [],
                 action: () => {
@@ -1156,15 +1156,15 @@
         }), e.length > 1 && r.push({
             label: "clear_selection",
             labelArgs: [],
             actionStr: "clear",
             icon: "mdi-cancel"
         }), r
     },
-    Ni = Re({
+    Ni = Be({
         __name: "MediaItemContextMenu",
         props: {
             items: {},
             parentItem: {
                 default: void 0
             },
             modelValue: {
@@ -1187,20 +1187,20 @@
         setup(e, {
             emit: t
         }) {
             const i = e,
                 {
                     t: r
                 } = Ee(),
-                l = H([]),
-                m = H([]),
-                s = H(""),
-                n = H([]),
-                o = H(!1),
-                f = H("");
+                l = K([]),
+                m = K([]),
+                s = K(""),
+                n = K([]),
+                o = K(!1),
+                f = K("");
             ot(() => i.modelValue, d => {
                 d && $()
             });
             const $ = async function() {
                 if (o.value = !1, n.value = [], !i.items) return;
                 i.items.length === 1 ? s.value = i.items[0].name : s.value = r("items_selected", [i.items.length]).toString(), te.selectedPlayer && te.selectedPlayer.available ? m.value = mi(i.items, i.parentItem) : m.value = [];
                 let d = i.items[0],
@@ -1218,18 +1218,18 @@
                 l.value = We(i.items, i.parentItem, r), C()
             }, C = async function() {
                 n.value = [];
                 const d = await w.getLibraryPlaylists();
                 for (const h of d.items) h.is_editable && !(i.parentItem && i.parentItem.media_type === A.PLAYLIST && h.item_id === i.parentItem.item_id) && n.value.push(h)
             }, M = function(d) {
                 w.addPlaylistTracks(d.item_id, i.items.map(h => h.uri)), k()
-            }, R = async function(d) {
+            }, B = async function(d) {
                 const h = await w.createPlaylist(f.value, d);
                 M(h)
-            }, U = async function(d) {
+            }, H = async function(d) {
                 d.actionStr == "add_playlist" ? o.value = !0 : d.actionStr == "clear" ? (t("clear"), k()) : d.action && d.actionStr == "play" ? (d.action(), t("clear"), k()) : d.action && (k(), d.action())
             }, k = function() {
                 i.items.length == 1 && t("clear"), t("update:modelValue", !1)
             }, _ = ge(() => {
                 var h, c;
                 const d = [];
                 for (const a in (h = w) == null ? void 0 : h.players) {
@@ -1261,23 +1261,23 @@
                             icon: "mdi-play-circle-outline"
                         }), o.value ? (u(), V(Ve, {
                             key: 0,
                             style: {
                                 "padding-left": "10px"
                             }
                         }, {
-                            default: p(() => [B("b", null, S(d.$t("add_playlist")), 1), d.$vuetify.display.mobile ? I("", !0) : (u(), g("span", ai, " | " + S(s.value), 1))]),
+                            default: p(() => [R("b", null, S(d.$t("add_playlist")), 1), d.$vuetify.display.mobile ? I("", !0) : (u(), g("span", ai, " | " + S(s.value), 1))]),
                             _: 1
                         })) : (u(), V(Ve, {
                             key: 1,
                             style: {
                                 "padding-left": "10px"
                             }
                         }, {
-                            default: p(() => [B("b", null, S(s.value), 1)]),
+                            default: p(() => [R("b", null, S(s.value), 1)]),
                             _: 1
                         })), y(ne, {
                             icon: "mdi-close",
                             dark: "",
                             onClick: h[0] || (h[0] = c => k())
                         })]),
                         _: 1
@@ -1296,22 +1296,22 @@
                                 })
                             }, null, 8, ["label", "model-value", "items"]), y(de, null, {
                                 default: p(() => [(u(!0), g(X, null, J(m.value, a => (u(), g("div", {
                                     key: a.label
                                 }, [y(Q, {
                                     title: d.$t(a.label, a.labelArgs),
                                     density: "default",
-                                    onClick: P => U(a)
+                                    onClick: P => H(a)
                                 }, {
                                     prepend: p(() => [y(ze, {
                                         style: {
                                             "padding-right": "10px"
                                         }
                                     }, {
-                                        default: p(() => [y(N, {
+                                        default: p(() => [y(U, {
                                             icon: a.icon
                                         }, null, 8, ["icon"])]),
                                         _: 2
                                     }, 1024)]),
                                     _: 2
                                 }, 1032, ["title", "onClick"])]))), 128))]),
                                 _: 1
@@ -1335,22 +1335,22 @@
                             _: 1
                         }), y(de, null, {
                             default: p(() => [(u(!0), g(X, null, J(l.value, c => (u(), g("div", {
                                 key: c.label
                             }, [y(Q, {
                                 title: d.$t(c.label, c.labelArgs),
                                 density: "default",
-                                onClick: a => U(c)
+                                onClick: a => H(c)
                             }, {
                                 prepend: p(() => [y(ze, {
                                     style: {
                                         "padding-right": "10px"
                                     }
                                 }, {
-                                    default: p(() => [y(N, {
+                                    default: p(() => [y(U, {
                                         icon: c.icon
                                     }, null, 8, ["icon"])]),
                                     _: 2
                                 }, 1024)]),
                                 _: 2
                             }, 1032, ["title", "onClick"])]))), 128))]),
                             _: 1
@@ -1363,22 +1363,22 @@
                             default: p(() => [(u(!0), g(X, null, J(n.value, c => (u(), g("div", {
                                 key: c.item_id
                             }, [y(Q, {
                                 ripple: "",
                                 density: "default",
                                 onClick: a => M(c)
                             }, {
-                                prepend: p(() => [B("div", ui, [y(De, {
+                                prepend: p(() => [R("div", ui, [y(De, {
                                     item: c,
                                     size: 50,
                                     width: "50px",
                                     height: "50px"
                                 }, null, 8, ["item"])])]),
-                                title: p(() => [B("div", null, S(c.name), 1)]),
-                                subtitle: p(() => [B("div", null, S(c.owner), 1)]),
+                                title: p(() => [R("div", null, S(c.name), 1)]),
+                                subtitle: p(() => [R("div", null, S(c.owner), 1)]),
                                 append: p(() => [c.provider_mappings ? (u(), V(fe, {
                                     key: 0,
                                     domain: c.provider_mappings[0].provider_domain,
                                     size: 20
                                 }, null, 8, ["domain"])) : I("", !0)]),
                                 _: 2
                             }, 1032, ["onClick"])]))), 128)), (u(!0), g(X, null, J(b(w).providers, c => (u(), g("div", {
@@ -1395,16 +1395,16 @@
                                     label: d.$t("create_playlist", [c.name]),
                                     "append-icon": "mdi-playlist-plus",
                                     variant: "plain",
                                     "hide-details": "",
                                     "onUpdate:modelValue": h[2] || (h[2] = a => {
                                         f.value = a
                                     }),
-                                    "onClick:append": a => R(c.instance_id),
-                                    onKeydown: at(a => R(c.instance_id), ["enter"])
+                                    "onClick:append": a => B(c.instance_id),
+                                    onKeydown: at(a => B(c.instance_id), ["enter"])
                                 }, null, 8, ["label", "onClick:append", "onKeydown"])]),
                                 _: 2
                             }, 1024)])) : I("", !0)]))), 128))]),
                             _: 1
                         })]),
                         _: 1
                     })) : I("", !0)]),
@@ -1463,15 +1463,15 @@
     zi = {
         class: "text-caption",
         style: {
             "padding-right": "10px",
             "padding-left": "10px"
         }
     },
-    Ai = Re({
+    Ai = Be({
         __name: "ListviewItem",
         props: {
             item: {},
             showTrackNumber: {
                 type: Boolean,
                 default: !0
             },
@@ -1527,15 +1527,15 @@
         }) {
             const i = e,
                 {
                     t: r
                 } = Ee(),
                 l = ge(() => {
                     for (const s of i.item.provider_mappings)
-                        if (s.audio_format.content_type != null && [ie.DSF, ie.FLAC, ie.AIFF, ie.WAV].includes(s.audio_format.content_type) && (s.audio_format.sample_rate > 48e3 || s.audio_format.bit_depth > 16)) return `${s.audio_format.sample_rate/1e3}kHz ${s.audio_format.bit_depth} bits`;
+                        if (s.audio_format.content_type != null && [se.DSF, se.FLAC, se.AIFF, se.WAV].includes(s.audio_format.content_type) && (s.audio_format.sample_rate > 48e3 || s.audio_format.bit_depth > 16)) return `${s.audio_format.sample_rate/1e3}kHz ${s.audio_format.bit_depth} bits`;
                     return ""
                 }),
                 m = function(s) {
                     var n;
                     if (s.media_type == A.FOLDER || !i.item.provider_mappings) return !0;
                     for (const o of s.provider_mappings)
                         if (o.available && ((n = w.providers[o.provider_instance]) != null && n.available)) return !0;
@@ -1544,98 +1544,98 @@
             return (s, n) => {
                 const o = Le("hold");
                 return u(), g("div", null, [Oe((u(), V(Q, {
                     link: "",
                     disabled: !m(s.item) || s.isDisabled,
                     onClick: n[5] || (n[5] = Y(f => t("click", s.item), ["stop"])),
                     onContextmenu: n[6] || (n[6] = Y(f => t("menu", s.item), ["right", "prevent"])),
-                    "context-menu-items": s.showMenu ? b(We)([s.item]) : []
+                    "context-menu-items": s.showMenu ? b(We)([s.item], s.parentItem) : []
                 }, {
                     prepend: p(() => [s.showCheckboxes ? (u(), g("div", fi, [y(ri, {
                         "model-value": s.isSelected,
                         onClick: n[0] || (n[0] = Y(() => {}, ["stop"])),
                         "onUpdate:modelValue": n[1] || (n[1] = f => {
                             t("select", s.item, f)
                         })
                     }, null, 8, ["model-value"])])) : s.item.media_type == b(A).FOLDER ? (u(), g("div", pi, [y(ne, {
                         variant: "plain",
                         icon: ""
                     }, {
-                        default: p(() => [y(N, {
+                        default: p(() => [y(U, {
                             icon: "mdi-folder",
                             size: "60",
                             style: {
                                 align: "center"
                             }
                         })]),
                         _: 1
                     })])) : (u(), g("div", hi, [y(De, {
                         height: "50",
                         width: "50",
                         item: s.item
                     }, null, 8, ["item"])]))]),
-                    title: p(() => [s.item.media_type == b(A).FOLDER ? (u(), g("span", yi, [B("span", null, S(b(ut)(s.item, b(r))), 1)])) : (u(), g("span", vi, [F(S(s.item.name) + " ", 1), "version" in s.item && s.item.version ? (u(), g("span", bi, "(" + S(s.item.version) + ")", 1)) : I("", !0)])), s.item && s.item.metadata ? (u(), V(b(Ie), {
+                    title: p(() => [s.item.media_type == b(A).FOLDER ? (u(), g("span", yi, [R("span", null, S(b(ut)(s.item, b(r))), 1)])) : (u(), g("span", vi, [F(S(s.item.name) + " ", 1), "version" in s.item && s.item.version ? (u(), g("span", bi, "(" + S(s.item.version) + ")", 1)) : I("", !0)])), s.item && s.item.metadata ? (u(), V(b(Ie), {
                         key: 2,
                         location: "bottom"
                     }, {
                         activator: p(({
                             props: f
-                        }) => [b(dt)(s.item.metadata.explicit || !1) ? (u(), V(N, x({
+                        }) => [b(dt)(s.item.metadata.explicit || !1) ? (u(), V(U, Z({
                             key: 0
                         }, f, {
                             icon: "mdi-alpha-e-box",
                             width: "35"
                         }), null, 16)) : I("", !0)]),
-                        default: p(() => [B("span", null, S(s.$t("tooltip.explicit")), 1)]),
+                        default: p(() => [R("span", null, S(s.$t("tooltip.explicit")), 1)]),
                         _: 1
                     })) : I("", !0)]),
                     subtitle: p(() => [s.item.media_type == b(A).TRACK ? (u(), g("div", gi, [y(oi, null, {
                         default: p(() => ["artists" in s.item ? (u(), V(q, {
                             key: 0
                         }, {
-                            default: p(() => [F(S(b(se)(s.item.artists, 2)), 1)]),
+                            default: p(() => [F(S(b(ie)(s.item.artists, 2)), 1)]),
                             _: 1
                         })) : I("", !0), s.showAlbum && "album" in s.item && s.item.album ? (u(), V(q, {
                             key: 1
                         }, {
                             default: p(() => [F(" • " + S(s.item.album.name), 1)]),
                             _: 1
                         })) : I("", !0), "disc_number" in s.item && s.item.disc_number && s.showDiscNumber ? (u(), V(q, {
                             key: 2
                         }, {
-                            default: p(() => [y(N, {
+                            default: p(() => [y(U, {
                                 style: {
                                     "margin-left": "5px"
                                 },
                                 icon: "md:album"
                             }), F(" " + S(s.item.disc_number), 1)]),
                             _: 1
                         })) : I("", !0), "track_number" in s.item && s.item.track_number && s.showTrackNumber ? (u(), V(q, {
                             key: 3
                         }, {
-                            default: p(() => [y(N, {
+                            default: p(() => [y(U, {
                                 style: {
                                     "margin-left": "5px"
                                 },
                                 icon: "mdi-music-circle-outline"
                             }), F(" " + S(s.item.track_number), 1)]),
                             _: 1
                         })) : "position" in s.item && s.item.position && s.showPosition ? (u(), V(q, {
                             key: 4
                         }, {
-                            default: p(() => [y(N, {
+                            default: p(() => [y(U, {
                                 style: {
                                     "margin-left": "5px"
                                 },
                                 icon: "mdi-music-circle-outline"
                             }), F(" " + S(s.item.position), 1)]),
                             _: 1
                         })) : I("", !0)]),
                         _: 1
-                    })])) : s.item.media_type == b(A).ALBUM && "artists" in s.item && s.item.artists && "year" in s.item && s.item.year && "album_type" in s.item ? (u(), g("div", _i, S(s.$t("album_type." + s.item.album_type)) + " • " + S(b(se)(s.item.artists)) + " • " + S(s.item.year), 1)) : s.item.media_type == b(A).ALBUM && "artists" in s.item && s.item.artists && "album_type" in s.item ? (u(), g("div", Si, S(s.$t("album_type." + s.item.album_type)) + " • " + S(b(se)(s.item.artists)), 1)) : "artists" in s.item && s.item.artists ? (u(), g("div", wi, S(b(se)(s.item.artists)), 1)) : "owner" in s.item && s.item.owner ? (u(), g("div", ki, S(s.item.owner), 1)) : I("", !0), s.item.media_type == b(A).RADIO && s.item.metadata.description ? (u(), g("div", Ii, S(s.item.metadata.description), 1)) : I("", !0)]),
+                    })])) : s.item.media_type == b(A).ALBUM && "artists" in s.item && s.item.artists && "year" in s.item && s.item.year && "album_type" in s.item ? (u(), g("div", _i, S(s.$t("album_type." + s.item.album_type)) + " • " + S(b(ie)(s.item.artists)) + " • " + S(s.item.year), 1)) : s.item.media_type == b(A).ALBUM && "artists" in s.item && s.item.artists && "album_type" in s.item ? (u(), g("div", Si, S(s.$t("album_type." + s.item.album_type)) + " • " + S(b(ie)(s.item.artists)), 1)) : "artists" in s.item && s.item.artists ? (u(), g("div", wi, S(b(ie)(s.item.artists)), 1)) : "owner" in s.item && s.item.owner ? (u(), g("div", ki, S(s.item.owner), 1)) : I("", !0), s.item.media_type == b(A).RADIO && s.item.metadata.description ? (u(), g("div", Ii, S(s.item.metadata.description), 1)) : I("", !0)]),
                     append: p(() => [l.value ? (u(), V(At, {
                         key: 0,
                         src: b(mt),
                         width: "30",
                         class: me(s.$vuetify.theme.current.dark ? "hiresicondark" : "hiresicon")
                     }, {
                         default: p(() => [y(b(Ie), {
@@ -1646,28 +1646,28 @@
                             _: 1
                         })]),
                         _: 1
                     }, 8, ["src", "class"])) : I("", !0), b(ae)("bp2") && s.showProvider ? (u(), V(fe, {
                         key: 1,
                         domain: s.item.media_type == b(A).PLAYLIST ? s.item.provider_mappings[0].provider_domain : s.item.provider,
                         size: 24
-                    }, null, 8, ["domain"])) : I("", !0), b(ae)("bp3") && "favorite" in s.item && s.showFavorite && !s.$vuetify.display.mobile ? (u(), g("div", Vi, [y(ne, x({
+                    }, null, 8, ["domain"])) : I("", !0), b(ae)("bp3") && "favorite" in s.item && s.showFavorite && !s.$vuetify.display.mobile ? (u(), g("div", Vi, [y(ne, Z({
                         variant: "plain",
                         ripple: ""
                     }, i, {
                         icon: s.item.favorite ? "mdi-heart" : "mdi-heart-outline",
                         onClick: [n[2] || (n[2] = f => b(w).toggleFavorite(s.item)), n[3] || (n[3] = Y(() => {}, ["prevent"])), n[4] || (n[4] = Y(() => {}, ["stop"]))],
                         title: s.$t("tooltip.favorite")
-                    }), null, 16, ["icon", "title"])])) : I("", !0), s.showDuration && s.item.media_type == b(A).TRACK && "duration" in s.item && s.item.duration != null && b(ae)("bp0") ? (u(), g("div", $i, [B("div", null, [B("span", zi, S(b(ct)(s.item.duration)), 1)])])) : I("", !0)]),
+                    }), null, 16, ["icon", "title"])])) : I("", !0), s.showDuration && s.item.media_type == b(A).TRACK && "duration" in s.item && s.item.duration != null && b(ae)("bp0") ? (u(), g("div", $i, [R("div", null, [R("span", zi, S(b(ct)(s.item.duration)), 1)])])) : I("", !0)]),
                     _: 1
                 }, 8, ["disabled", "context-menu-items"])), [
                     [o, () => t("menu", s.item)]
                 ])])
             }
         }
     });
 const Ui = ft(Ai, [
-    ["__scopeId", "data-v-f28c82e3"]
+    ["__scopeId", "data-v-d473232c"]
 ]);
 export {
-    Ui as L, ri as V, Ni as _, mi as a, oi as b, q as c, We as g, j as i, je as s
+    Ui as L, ri as V, Ni as _, mi as a, oi as b, q as c, We as g, G as i, je as s
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb-24a77af5.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,64 +1,64 @@
 import {
     m as P,
     a as U,
-    f as X,
     c as O,
+    f as X,
     V as L,
     b as T
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     p as V,
     as as Z,
     g as x,
     f as G,
     al as K,
     c as l,
     r as M,
-    k as w,
     j as u,
+    k as w,
     l as N,
-    B as C,
-    O as R,
     q as h,
     v as I,
     x as c,
     L as m,
     N as g,
     M as b,
     K as d,
     A as F,
     X as B,
-    y as J,
+    y as C,
     aA as f,
+    O as R,
+    B as J,
     ax as Q,
     w as W,
     aa as z
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     i as j,
     j as q
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     a as _
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     a as $
-} from "./VDialog-5f240a62.js";
+} from "./VDialog-93a2100b.js";
 import {
     V as ee,
     c as te,
     b as ie
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     V as ae
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     a as Ae
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 const re = V({
         id: String,
         text: String,
         ...Z(P({
             closeOnBack: !1,
             location: "end",
             locationStrategy: "connected",
@@ -174,15 +174,15 @@
     Me = new URL("" + new URL("hires-438c7046.png", import.meta.url).href, self.location).href,
     ke = new URL("" + new URL("cover_dark-75402cd0.png", import.meta.url).href, self.location).href,
     ve = new URL("" + new URL("cover_light-b832ae9e.png", import.meta.url).href, self.location).href,
     Ne = N({
         __name: "QualityDetailsBtn",
         setup(e) {
             const t = l(() => {
-                    if (C.selectedPlayer) return R.queues[C.selectedPlayer.active_source]
+                    if (J.selectedPlayer) return R.queues[J.selectedPlayer.active_source]
                 }),
                 a = l(() => {
                     var i, o;
                     return (o = (i = t.value) == null ? void 0 : i.current_item) == null ? void 0 : o.streamdetails
                 }),
                 A = function(i) {
                     return i == f.AAC ? de : i == f.FLAC ? he : i == f.MP3 || i == f.MPEG ? H : i == f.OGG ? Re : i == f.M4A ? pe : fe
@@ -238,21 +238,21 @@
                                     "margin-right": "5px"
                                 }
                             }, null, 8, ["domain"]), d(" " + g(((r = F(R).providerManifests[a.value.provider]) == null ? void 0 : r.name) || ((n = F(R).providers[a.value.provider]) == null ? void 0 : n.name)), 1)]), m("div", ce, [m("img", {
                                 height: "30",
                                 width: "50",
                                 src: A(a.value.audio_format.content_type),
                                 style: B(i.$vuetify.theme.current.dark ? "object-fit: contain;" : "object-fit: contain;filter: invert(100%);")
-                            }, null, 12, ue), d(" " + g(a.value.audio_format.sample_rate / 1e3) + " kHz / " + g(a.value.audio_format.bit_depth) + " bits ", 1)]), t.value && t.value.crossfade_enabled ? (h(), J("div", ge, [m("img", {
+                            }, null, 12, ue), d(" " + g(a.value.audio_format.sample_rate / 1e3) + " kHz / " + g(a.value.audio_format.bit_depth) + " bits ", 1)]), t.value && t.value.crossfade_enabled ? (h(), C("div", ge, [m("img", {
                                 height: "30",
                                 width: "50",
                                 contain: "",
                                 src: ne,
                                 style: B(i.$vuetify.theme.current.dark ? "object-fit: contain;" : "object-fit: contain;filter: invert(100%);")
-                            }, null, 4), d(" " + g(i.$t("crossfade_enabled")), 1)])) : b("", !0), a.value.gain_correct ? (h(), J("div", me, [m("img", {
+                            }, null, 4), d(" " + g(i.$t("crossfade_enabled")), 1)])) : b("", !0), a.value.gain_correct ? (h(), C("div", me, [m("img", {
                                 height: "30",
                                 width: "50",
                                 contain: "",
                                 src: oe,
                                 style: B(i.$vuetify.theme.current.dark ? "object-fit: contain;" : "object-fit: contain;filter: invert(100%);")
                             }, null, 4), d(" " + g(a.value.gain_correct) + " dB ", 1)])) : b("", !0)]
                         }),
@@ -365,9 +365,9 @@
                     })])]),
                     _: 1
                 }, 8, ["style", "cover", "src", "aspect-ratio", "lazy-src"])
             }
         }
     });
 export {
-    He as V, Se as _, ve as a, Ne as b, fe as c, Me as d, Fe as g, ke as i
+    He as V, Se as _, Ne as a, ve as b, fe as c, Me as d, Fe as g, ke as i
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,54 +1,54 @@
 import {
     l as C,
     r as V,
     c as g,
-    aA as d,
     a9 as I,
     Q as $,
     q as a,
     v as s,
     x as t,
     j as o,
     M as l,
     K as n,
     N as r,
     A as f,
     a7 as S,
     aj as N,
     W as T,
-    ai as A
-} from "./index-e9211ef1.js";
+    ah as A,
+    aA as d
+} from "./index-ade73b84.js";
 import {
     _ as B,
     d as D,
     V as _
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
 import {
     L
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     c as F
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     V as M,
     b as z,
     c as p
-} from "./ListviewItem-b7a4258b.js";
+} from "./ListviewItem-2bd74fad.js";
 import {
     c as H,
     d as b,
     b as j
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     V as c
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     a as P
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 const J = C({
     __name: "PanelviewItem",
     props: {
         item: {},
         size: {
             default: 200
         },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/PlayerQueue-29876489.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/PlayerQueue-7ca94b07.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,77 +1,77 @@
 import {
     l as Y,
     J as Z,
     I as Q,
     r as M,
     c as w,
-    B as k,
-    O as n,
     o as ee,
+    O as n,
     af as x,
     b as le,
+    B as k,
     w as te,
     q as p,
     y as U,
     j as t,
     x as a,
     K as $,
     N as d,
     v as f,
     L as v,
     M as _,
     A as V,
     k as J,
-    ai as h,
+    ah as h,
     a2 as ue,
-    U as ae
-} from "./index-e9211ef1.js";
+    S as ae
+} from "./index-ade73b84.js";
 import {
     L as oe,
     s as ie
-} from "./ListviewItem-b7a4258b.js"; /* empty css                             */
+} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
 import {
     C as ne,
     L as g
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     A as O
-} from "./Alert-55091fd0.js";
+} from "./Alert-4d78da02.js";
 import {
     V as P,
     a as se
-} from "./VTabs-13127e50.js";
+} from "./VTabs-21d8affa.js";
 import {
     V as F
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
 import {
     l as A,
     V as q
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     a as re,
     c as de
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as me,
     b as G
-} from "./VToolbar-daf2b89f.js";
+} from "./VToolbar-806969a3.js";
 import {
     V as pe
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     a as y
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     V as C
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     V as ve
-} from "./VDialog-5f240a62.js";
-import "./VSelect-04a129eb.js"; /* empty css              */
+} from "./VDialog-93a2100b.js";
+import "./VSelect-a66ffc02.js"; /* empty css              */
 const fe = v("br", null, null, -1),
     _e = {
         key: 0
     },
     be = {
         key: 0
     },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Players-b1f01106.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Players-5c99fe5e.js`

 * *Files 10% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     C as M,
     L as T,
     a as z
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     B as b
-} from "./Button-59559304.js";
+} from "./Button-4a781169.js";
 import {
     V as f
-} from "./VBtn-68784d55.js";
-import "./VMenu-bc0cce60.js";
-import "./VDivider-336c24cd.js";
-import "./VListItem-230d1393.js"; /* empty css              */
+} from "./VBtn-61e39030.js";
+import "./VMenu-ccc026f2.js";
+import "./VDivider-adefbf87.js";
+import "./VListItem-f848c028.js"; /* empty css              */
 const O = {
         class: "line-clamp-1"
     },
     R = {
         class: "line-clamp-1"
     },
     K = w({
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Providers-a361876b.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Providers-65d3d824.js`

 * *Files 3% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     C as I,
     L as A,
     a as S,
     _ as Y
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     B as b
-} from "./Button-59559304.js";
+} from "./Button-4a781169.js";
 import {
     A as Z
-} from "./Alert-55091fd0.js";
+} from "./Alert-4d78da02.js";
 import {
     a as B
-} from "./VCard-138864fc.js";
+} from "./VCard-f3e11b51.js";
 import {
     V as ee
-} from "./VToolbar-daf2b89f.js";
+} from "./VToolbar-806969a3.js";
 import {
     b as te
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 import {
     l as ne,
     V as g
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     V as ae
-} from "./VDivider-336c24cd.js";
-import "./VListItem-230d1393.js"; /* empty css              */
+} from "./VDivider-adefbf87.js";
+import "./VListItem-f848c028.js"; /* empty css              */
 const ie = _ => (W("data-v-273ae240"), _ = _(), X(), _),
     se = {
         class: "line-clamp-1"
     },
     oe = ie(() => p("br", null, null, -1)),
     re = {
         class: "line-clamp-1"
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Search-b8c39f87.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Search-f31ee239.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 import {
     _ as q,
     L as A,
     s as G
-} from "./ListviewItem-b7a4258b.js"; /* empty css                             */
+} from "./ListviewItem-2bd74fad.js"; /* empty css                             */
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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     _ as ee
-} from "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js";
+} from "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js";
 import {
     C as te
-} from "./Container-349a0ac0.js";
+} from "./Container-282a676b.js";
 import {
     V as ae
-} from "./VSelect-04a129eb.js";
+} from "./VSelect-a66ffc02.js";
 import {
     b as le,
     a as se
-} from "./VDialog-5f240a62.js";
+} from "./VDialog-93a2100b.js";
 import {
     V as re,
     a as oe
-} from "./VRow-e8f3e51e.js";
+} from "./VRow-74a0e5a5.js";
 import {
     V as ue
-} from "./VToolbar-daf2b89f.js";
+} from "./VToolbar-806969a3.js";
 import {
     V as ie
-} from "./VSpacer-bdf2f653.js";
+} from "./VSpacer-159b0383.js";
 import {
     V as ne
-} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js";
+} from "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js";
 import {
     l as ve,
     k as me
-} from "./VBtn-68784d55.js";
-import "./VDivider-336c24cd.js";
-import "./VCard-138864fc.js";
-import "./VListItem-230d1393.js";
-import "./VMenu-bc0cce60.js"; /* empty css              */
+} from "./VBtn-61e39030.js";
+import "./VDivider-adefbf87.js";
+import "./VCard-f3e11b51.js";
+import "./VListItem-f848c028.js";
+import "./VMenu-ccc026f2.js"; /* empty css              */
 const fe = {
         key: 2
     },
     ce = {
         style: {
             "margin-left": "15px"
         }
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/Settings-244fcb0f.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/Settings-f159e60c.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,41 @@
 import {
-    l as d,
-    I as m,
+    l as m,
+    I as d,
     c as v,
     P as f,
     q as l,
     y as _,
     j as e,
     x as a,
     K as o,
     N as s,
     T as g,
     v as y,
     R as V
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     V as n,
     a as T
-} from "./VTabs-13127e50.js";
+} from "./VTabs-21d8affa.js";
 import {
     V as b
-} from "./VDivider-336c24cd.js";
-import "./VBtn-68784d55.js";
-const w = d({
+} from "./VDivider-adefbf87.js";
+import "./VBtn-61e39030.js";
+const B = m({
     __name: "Settings",
     setup(C) {
-        const i = m(),
+        const i = d(),
             u = v(() => {
                 var t, r;
                 return (t = i.currentRoute.value.name) != null && t.toString().includes("player") ? "players" : (r = i.currentRoute.value.name) != null && r.toString().includes("core") ? "core" : "providers"
             });
         return (t, r) => {
             const c = f("router-view");
             return l(), _("section", null, [e(T, {
-                "hide-slider": "",
                 "model-value": u.value,
                 "align-tabs": "end"
             }, {
                 default: a(() => [e(n, {
                     value: "providers",
                     to: {
                         name: "providersettings"
@@ -76,10 +75,10 @@
                 }, 1024)]),
                 _: 1
             })])
         }
     }
 });
 export {
-    w as
+    B as
     default
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBadge-9c063078.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-9c063078.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBadge-9fa94f29.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBadge-12aff0c7.js`

 * *Files 9% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     m as D,
     M as F
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 const Q = B({
         bordered: Boolean,
         color: String,
         content: [Number, String],
         dot: Boolean,
         floating: Boolean,
         icon: S,
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBtn-68784d55.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-61e39030.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -7,17 +7,17 @@
     b as q,
     w as K,
     b7 as me,
     b1 as et,
     g as E,
     at as tt,
     i as Be,
+    b5 as Ie,
     c as u,
     bf as A,
-    b5 as Ie,
     bg as ge,
     a$ as P,
     a as h,
     av as ne,
     m as D,
     d as G,
     bh as nt,
@@ -46,15 +46,15 @@
     s as bt,
     bb as yt,
     H as Ct,
     u as Le,
     T as pt,
     Q as St,
     a9 as kt
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 const Te = ["top", "bottom"],
     _t = ["start", "end", "left", "right"];
 
 function wt(e, t) {
     let [a, n] = e.split(" ");
     return n || (n = j(Te, a) ? "start" : j(_t, a) ? "top" : "center"), {
         side: Ce(a, t),
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VBtn-76f512af.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VBtn-76f512af.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VCard-103d8462.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-103d8462.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VCard-138864fc.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VCard-f3e11b51.js`

 * *Files 1% similar despite different names*

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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     e as p,
     a as A,
     b as ke
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 const ye = b()({
         name: "VCardActions",
         props: y(),
         setup(e, i) {
             let {
                 slots: t
             } = i;
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDialog-28e4e64e.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-28e4e64e.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDialog-5f240a62.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDialog-93a2100b.js`

 * *Files 1% similar despite different names*

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     f as Pe,
     e as Ae
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     a as ee,
     m as je,
     M as qe
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     m as He,
     i as Xe,
     a as Qe,
-    f as We,
-    c as ae
-} from "./VMenu-bc0cce60.js";
+    c as ae,
+    f as We
+} from "./VMenu-ccc026f2.js";
 const de = Symbol.for("vuetify:v-chip-group"),
     Ye = A({
         column: Boolean,
         filter: Boolean,
         valueComparator: {
             type: Function,
             default: fe
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDivider-336c24cd.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-adefbf87.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,22 +5,22 @@
     aD as x,
     p,
     ba as _,
     m as C,
     d as B,
     t as P,
     c as V,
-    a as m,
-    j as E
-} from "./index-e9211ef1.js";
+    j as E,
+    a as m
+} from "./index-ade73b84.js";
 import {
     a as L,
     y as $,
     i as A
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 class y {
     constructor(r) {
         let {
             x: s,
             y: n,
             width: o,
             height: a
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VDivider-bc1524a3.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VDivider-bc1524a3.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-16e67e58.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VExpansionPanel-67038b00.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VExpansionPanel-75456689.js`

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     d as qe,
     c as Ke
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     g as Ge,
     m as Ue,
     u as Qe,
     c as ue,
     f as Xe
-} from "./VDialog-5f240a62.js";
+} from "./VDialog-93a2100b.js";
 import {
     d as Se,
     e as Ye
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 const le = Symbol.for("vuetify:v-slider");
 
 function We(e, a, t) {
     const l = t === "vertical",
         i = a.getBoundingClientRect(),
         m = "touches" in e ? e.touches[0] : e;
     return l ? m.clientY - (i.top + i.height / 2) : m.clientX - (i.left + i.width / 2)
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VGrid-b9c72806.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VGrid-b9c72806.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VListItem-230d1393.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-f848c028.js`

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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 
 function Pe(e) {
     let r = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : "div",
         a = arguments.length > 2 ? arguments[2] : void 0;
     return M()({
         name: a ?? Ue(qe(e.replace(/__/g, "-"))),
         props: {
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VListItem-b9e24cb0.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VListItem-b9e24cb0.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VMenu-b930657a.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-b930657a.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VMenu-bc0cce60.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VMenu-ccc026f2.js`

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
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
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
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
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 const te = new WeakMap;
 
 function en(e, n) {
     Object.keys(n).forEach(t => {
         if (He(t)) {
             const o = We(t),
                 a = te.get(e);
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VRow-e8f3e51e.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VRow-74a0e5a5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 /* empty css              */
 import {
     a as C,
     d as S
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     aB as i,
     aC as u,
     p as b,
     g as k,
     c as N,
     aD as j
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 const V = (() => i.reduce((t, a) => (t[a] = {
         type: [Boolean, String, Number],
         default: !1
     }, t), {}))(),
     v = (() => i.reduce((t, a) => {
         const e = "offset" + u(a);
         return t[e] = {
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VSelect-04a129eb.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-a66ffc02.js`

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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     e as nl,
     n as al,
     b as ol,
     s as il,
     f as ul
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
 import {
     m as pe,
     M as Cl,
     I as xl,
     V as me
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 import {
     f as we,
     g as kl,
     u as Be,
     h as Il,
     m as Sl,
     c as ye,
     i as Pl,
     a as _l
-} from "./VDialog-5f240a62.js";
+} from "./VDialog-93a2100b.js";
 import {
     f as Fe,
     g as pl,
     h as wl,
     i as Bl,
     j as Fl,
     b as Tl,
     V as Rl
-} from "./VMenu-bc0cce60.js";
+} from "./VMenu-ccc026f2.js";
 const Te = Symbol.for("vuetify:selection-control-group"),
     Re = O({
         color: String,
         disabled: {
             type: Boolean,
             default: null
         },
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VSelect-45a454b3.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VSelect-45a454b3.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VTabs-13127e50.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-21d8affa.js`

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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     a as ee,
     b as we,
     s as Pe
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 
 function te(e) {
     const n = Math.abs(e);
     return Math.sign(e) * (n / ((1 / .501 - 2) * (1 - n) + 1))
 }
 
 function le(e) {
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VTabs-3cd3e980.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VTabs-3cd3e980.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VToolbar-222d6375.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-222d6375.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/VToolbar-daf2b89f.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/VToolbar-806969a3.js`

 * *Files 1% similar despite different names*

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
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 import {
     c as J
-} from "./VDivider-336c24cd.js";
+} from "./VDivider-adefbf87.js";
 import {
     b as K
-} from "./VListItem-230d1393.js";
+} from "./VListItem-f848c028.js";
 const L = V({
         text: String,
         ...x(),
         ...y()
     }, "VToolbarTitle"),
     M = k()({
         name: "VToolbarTitle",
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/cover_dark-75402cd0.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_dark-75402cd0.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/cover_light-b832ae9e.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/cover_light-b832ae9e.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/crossfade-ba51f69a.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/crossfade-ba51f69a.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/hires-438c7046.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/hires-438c7046.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/index-e9211ef1.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ade73b84.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -28,86 +28,86 @@
         if (o.ep) return;
         o.ep = !0;
         const a = n(o);
         fetch(o.href, a)
     }
 })();
 
-function hi(e, t) {
+function pi(e, t) {
     const n = Object.create(null),
         r = e.split(",");
     for (let o = 0; o < r.length; o++) n[r[o]] = !0;
     return t ? o => !!n[o.toLowerCase()] : o => !!n[o]
 }
 const de = {},
-    vn = [],
+    yn = [],
     mt = () => {},
     Hu = () => !1,
     xu = /^on[^a-z]/,
-    Xr = e => xu.test(e),
-    zi = e => e.startsWith("onUpdate:"),
+    Kr = e => xu.test(e),
+    hi = e => e.startsWith("onUpdate:"),
     ye = Object.assign,
-    bi = (e, t) => {
+    zi = (e, t) => {
         const n = e.indexOf(t);
         n > -1 && e.splice(n, 1)
     },
     Fu = Object.prototype.hasOwnProperty,
     ie = (e, t) => Fu.call(e, t),
     K = Array.isArray,
-    Tn = e => $r(e) === "[object Map]",
-    ml = e => $r(e) === "[object Set]",
+    vn = e => Xr(e) === "[object Map]",
+    ul = e => Xr(e) === "[object Set]",
     Q = e => typeof e == "function",
     be = e => typeof e == "string",
-    gi = e => typeof e == "symbol",
+    bi = e => typeof e == "symbol",
     me = e => e !== null && typeof e == "object",
-    dl = e => me(e) && Q(e.then) && Q(e.catch),
-    fl = Object.prototype.toString,
-    $r = e => fl.call(e),
-    Vu = e => $r(e).slice(8, -1),
-    _l = e => $r(e) === "[object Object]",
-    yi = e => be(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e,
-    kr = hi(",key,ref,ref_for,ref_key,onVnodeBeforeMount,onVnodeMounted,onVnodeBeforeUpdate,onVnodeUpdated,onVnodeBeforeUnmount,onVnodeUnmounted"),
-    Yr = e => {
+    ml = e => me(e) && Q(e.then) && Q(e.catch),
+    dl = Object.prototype.toString,
+    Xr = e => dl.call(e),
+    Vu = e => Xr(e).slice(8, -1),
+    fl = e => Xr(e) === "[object Object]",
+    gi = e => be(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e,
+    Cr = pi(",key,ref,ref_for,ref_key,onVnodeBeforeMount,onVnodeMounted,onVnodeBeforeUpdate,onVnodeUpdated,onVnodeBeforeUnmount,onVnodeUnmounted"),
+    $r = e => {
         const t = Object.create(null);
         return n => t[n] || (t[n] = e(n))
     },
     Uu = /-(\w)/g,
-    gt = Yr(e => e.replace(Uu, (t, n) => n ? n.toUpperCase() : "")),
+    gt = $r(e => e.replace(Uu, (t, n) => n ? n.toUpperCase() : "")),
     Wu = /\B([A-Z])/g,
-    nn = Yr(e => e.replace(Wu, "-$1").toLowerCase()),
-    ur = Yr(e => e.charAt(0).toUpperCase() + e.slice(1)),
-    Dr = Yr(e => e ? `on${ur(e)}` : ""),
-    Yn = (e, t) => !Object.is(e, t),
-    yo = (e, t) => {
+    nn = $r(e => e.replace(Wu, "-$1").toLowerCase()),
+    cr = $r(e => e.charAt(0).toUpperCase() + e.slice(1)),
+    kr = $r(e => e ? `on${cr(e)}` : ""),
+    $n = (e, t) => !Object.is(e, t),
+    go = (e, t) => {
         for (let n = 0; n < e.length; n++) e[n](t)
     },
-    Gr = (e, t, n) => {
+    Or = (e, t, n) => {
         Object.defineProperty(e, t, {
             configurable: !0,
             enumerable: !1,
             value: n
         })
     },
     ju = e => {
         const t = parseFloat(e);
         return isNaN(t) ? e : t
     },
     qu = e => {
         const t = be(e) ? Number(e) : NaN;
         return isNaN(t) ? e : t
     };
-let ca;
-const Bo = () => ca || (ca = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
+let la;
+const Lo = () => la || (la = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
 
-function vi(e) {
+function yi(e) {
     if (K(e)) {
         const t = {};
         for (let n = 0; n < e.length; n++) {
             const r = e[n],
-                o = be(r) ? Yu(r) : vi(r);
+                o = be(r) ? Yu(r) : yi(r);
             if (o)
                 for (const a in o) t[a] = o[a]
         }
         return t
     } else {
         if (be(e)) return e;
         if (me(e)) return e
@@ -123,39 +123,39 @@
         if (n) {
             const r = n.split(Xu);
             r.length > 1 && (t[r[0].trim()] = r[1].trim())
         }
     }), t
 }
 
-function Ti(e) {
+function vi(e) {
     let t = "";
     if (be(e)) t = e;
     else if (K(e))
         for (let n = 0; n < e.length; n++) {
-            const r = Ti(e[n]);
+            const r = vi(e[n]);
             r && (t += r + " ")
         } else if (me(e))
             for (const n in e) e[n] && (t += n + " ");
     return t.trim()
 }
 const Qu = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly",
-    Zu = hi(Qu);
+    Zu = pi(Qu);
 
-function pl(e) {
+function _l(e) {
     return !!e || e === ""
 }
-const qz = e => be(e) ? e : e == null ? "" : K(e) || me(e) && (e.toString === fl || !Q(e.toString)) ? JSON.stringify(e, hl, 2) : String(e),
-    hl = (e, t) => t && t.__v_isRef ? hl(e, t.value) : Tn(t) ? {
+const qz = e => be(e) ? e : e == null ? "" : K(e) || me(e) && (e.toString === dl || !Q(e.toString)) ? JSON.stringify(e, pl, 2) : String(e),
+    pl = (e, t) => t && t.__v_isRef ? pl(e, t.value) : vn(t) ? {
         [`Map(${t.size})`]: [...t.entries()].reduce((n, [r, o]) => (n[`${r} =>`] = o, n), {})
-    } : ml(t) ? {
+    } : ul(t) ? {
         [`Set(${t.size})`]: [...t.values()]
-    } : me(t) && !K(t) && !_l(t) ? String(t) : t;
+    } : me(t) && !K(t) && !fl(t) ? String(t) : t;
 let qe;
-class zl {
+class hl {
     constructor(t = !1) {
         this.detached = t, this._active = !0, this.effects = [], this.cleanups = [], this.parent = qe, !t && qe && (this.index = (qe.scopes || (qe.scopes = [])).push(this) - 1)
     }
     get active() {
         return this._active
     }
     run(t) {
@@ -186,237 +186,237 @@
                 o && o !== this && (this.parent.scopes[this.index] = o, o.index = this.index)
             }
             this.parent = void 0, this._active = !1
         }
     }
 }
 
-function bl(e) {
-    return new zl(e)
+function zl(e) {
+    return new hl(e)
 }
 
 function Ju(e, t = qe) {
     t && t.active && t.effects.push(e)
 }
 
 function em() {
     return qe
 }
 
 function tm(e) {
     qe && qe.cleanups.push(e)
 }
-const Si = e => {
+const Ti = e => {
         const t = new Set(e);
         return t.w = 0, t.n = 0, t
     },
-    gl = e => (e.w & Bt) > 0,
-    yl = e => (e.n & Bt) > 0,
+    bl = e => (e.w & Bt) > 0,
+    gl = e => (e.n & Bt) > 0,
     nm = ({
         deps: e
     }) => {
         if (e.length)
             for (let t = 0; t < e.length; t++) e[t].w |= Bt
     },
     rm = e => {
         const {
             deps: t
         } = e;
         if (t.length) {
             let n = 0;
             for (let r = 0; r < t.length; r++) {
                 const o = t[r];
-                gl(o) && !yl(o) ? o.delete(e) : t[n++] = o, o.w &= ~Bt, o.n &= ~Bt
+                bl(o) && !gl(o) ? o.delete(e) : t[n++] = o, o.w &= ~Bt, o.n &= ~Bt
             }
             t.length = n
         }
     },
-    Rr = new WeakMap;
-let xn = 0,
+    Gr = new WeakMap;
+let Hn = 0,
     Bt = 1;
-const No = 30;
+const Bo = 30;
 let st;
 const Zt = Symbol(""),
-    Ho = Symbol("");
-class Ai {
+    No = Symbol("");
+class Si {
     constructor(t, n = null, r) {
         this.fn = t, this.scheduler = n, this.active = !0, this.deps = [], this.parent = void 0, Ju(this, r)
     }
     run() {
         if (!this.active) return this.fn();
         let t = st,
             n = Gt;
         for (; t;) {
             if (t === this) return;
             t = t.parent
         }
         try {
-            return this.parent = st, st = this, Gt = !0, Bt = 1 << ++xn, xn <= No ? nm(this) : ua(this), this.fn()
+            return this.parent = st, st = this, Gt = !0, Bt = 1 << ++Hn, Hn <= Bo ? nm(this) : ca(this), this.fn()
         } finally {
-            xn <= No && rm(this), Bt = 1 << --xn, st = this.parent, Gt = n, this.parent = void 0, this.deferStop && this.stop()
+            Hn <= Bo && rm(this), Bt = 1 << --Hn, st = this.parent, Gt = n, this.parent = void 0, this.deferStop && this.stop()
         }
     }
     stop() {
-        st === this ? this.deferStop = !0 : this.active && (ua(this), this.onStop && this.onStop(), this.active = !1)
+        st === this ? this.deferStop = !0 : this.active && (ca(this), this.onStop && this.onStop(), this.active = !1)
     }
 }
 
-function ua(e) {
+function ca(e) {
     const {
         deps: t
     } = e;
     if (t.length) {
         for (let n = 0; n < t.length; n++) t[n].delete(e);
         t.length = 0
     }
 }
 let Gt = !0;
-const vl = [];
+const yl = [];
 
-function Dn() {
-    vl.push(Gt), Gt = !1
+function kn() {
+    yl.push(Gt), Gt = !1
 }
 
-function In() {
-    const e = vl.pop();
+function Dn() {
+    const e = yl.pop();
     Gt = e === void 0 ? !0 : e
 }
 
 function We(e, t, n) {
     if (Gt && st) {
-        let r = Rr.get(e);
-        r || Rr.set(e, r = new Map);
+        let r = Gr.get(e);
+        r || Gr.set(e, r = new Map);
         let o = r.get(n);
-        o || r.set(n, o = Si()), Tl(o)
+        o || r.set(n, o = Ti()), vl(o)
     }
 }
 
-function Tl(e, t) {
+function vl(e, t) {
     let n = !1;
-    xn <= No ? yl(e) || (e.n |= Bt, n = !gl(e)) : n = !e.has(st), n && (e.add(st), st.deps.push(e))
+    Hn <= Bo ? gl(e) || (e.n |= Bt, n = !bl(e)) : n = !e.has(st), n && (e.add(st), st.deps.push(e))
 }
 
 function Pt(e, t, n, r, o, a) {
-    const s = Rr.get(e);
+    const s = Gr.get(e);
     if (!s) return;
     let u = [];
     if (t === "clear") u = [...s.values()];
     else if (n === "length" && K(e)) {
         const c = Number(r);
         s.forEach((l, d) => {
             (d === "length" || d >= c) && u.push(l)
         })
     } else switch (n !== void 0 && u.push(s.get(n)), t) {
         case "add":
-            K(e) ? yi(n) && u.push(s.get("length")) : (u.push(s.get(Zt)), Tn(e) && u.push(s.get(Ho)));
+            K(e) ? gi(n) && u.push(s.get("length")) : (u.push(s.get(Zt)), vn(e) && u.push(s.get(No)));
             break;
         case "delete":
-            K(e) || (u.push(s.get(Zt)), Tn(e) && u.push(s.get(Ho)));
+            K(e) || (u.push(s.get(Zt)), vn(e) && u.push(s.get(No)));
             break;
         case "set":
-            Tn(e) && u.push(s.get(Zt));
+            vn(e) && u.push(s.get(Zt));
             break
     }
-    if (u.length === 1) u[0] && xo(u[0]);
+    if (u.length === 1) u[0] && Ho(u[0]);
     else {
         const c = [];
         for (const l of u) l && c.push(...l);
-        xo(Si(c))
+        Ho(Ti(c))
     }
 }
 
-function xo(e, t) {
+function Ho(e, t) {
     const n = K(e) ? e : [...e];
-    for (const r of n) r.computed && ma(r);
-    for (const r of n) r.computed || ma(r)
+    for (const r of n) r.computed && ua(r);
+    for (const r of n) r.computed || ua(r)
 }
 
-function ma(e, t) {
+function ua(e, t) {
     (e !== st || e.allowRecurse) && (e.scheduler ? e.scheduler() : e.run())
 }
 
 function om(e, t) {
     var n;
-    return (n = Rr.get(e)) == null ? void 0 : n.get(t)
+    return (n = Gr.get(e)) == null ? void 0 : n.get(t)
 }
-const im = hi("__proto__,__v_isRef,__isVue"),
-    Sl = new Set(Object.getOwnPropertyNames(Symbol).filter(e => e !== "arguments" && e !== "caller").map(e => Symbol[e]).filter(gi)),
-    am = Pi(),
-    sm = Pi(!1, !0),
-    lm = Pi(!0),
-    da = cm();
+const im = pi("__proto__,__v_isRef,__isVue"),
+    Tl = new Set(Object.getOwnPropertyNames(Symbol).filter(e => e !== "arguments" && e !== "caller").map(e => Symbol[e]).filter(bi)),
+    am = Ai(),
+    sm = Ai(!1, !0),
+    lm = Ai(!0),
+    ma = cm();
 
 function cm() {
     const e = {};
     return ["includes", "indexOf", "lastIndexOf"].forEach(t => {
         e[t] = function(...n) {
             const r = ee(this);
             for (let a = 0, s = this.length; a < s; a++) We(r, "get", a + "");
             const o = r[t](...n);
             return o === -1 || o === !1 ? r[t](...n.map(ee)) : o
         }
     }), ["push", "pop", "shift", "unshift", "splice"].forEach(t => {
         e[t] = function(...n) {
-            Dn();
+            kn();
             const r = ee(this)[t].apply(this, n);
-            return In(), r
+            return Dn(), r
         }
     }), e
 }
 
 function um(e) {
     const t = ee(this);
     return We(t, "has", e), t.hasOwnProperty(e)
 }
 
-function Pi(e = !1, t = !1) {
+function Ai(e = !1, t = !1) {
     return function(r, o, a) {
         if (o === "__v_isReactive") return !e;
         if (o === "__v_isReadonly") return e;
         if (o === "__v_isShallow") return t;
-        if (o === "__v_raw" && a === (e ? t ? Em : wl : t ? Ml : El).get(r)) return r;
+        if (o === "__v_raw" && a === (e ? t ? Em : Ml : t ? El : Pl).get(r)) return r;
         const s = K(r);
         if (!e) {
-            if (s && ie(da, o)) return Reflect.get(da, o, a);
+            if (s && ie(ma, o)) return Reflect.get(ma, o, a);
             if (o === "hasOwnProperty") return um
         }
         const u = Reflect.get(r, o, a);
-        return (gi(o) ? Sl.has(o) : im(o)) || (e || We(r, "get", o), t) ? u : Ae(u) ? s && yi(o) ? u : u.value : me(u) ? e ? kl(u) : Xe(u) : u
+        return (bi(o) ? Tl.has(o) : im(o)) || (e || We(r, "get", o), t) ? u : Ae(u) ? s && gi(o) ? u : u.value : me(u) ? e ? Cl(u) : Xe(u) : u
     }
 }
-const mm = Al(),
-    dm = Al(!0);
+const mm = Sl(),
+    dm = Sl(!0);
 
-function Al(e = !1) {
+function Sl(e = !1) {
     return function(n, r, o, a) {
         let s = n[r];
-        if (Mn(s) && Ae(s) && !Ae(o)) return !1;
-        if (!e && (!Lr(o) && !Mn(o) && (s = ee(s), o = ee(o)), !K(n) && Ae(s) && !Ae(o))) return s.value = o, !0;
-        const u = K(n) && yi(r) ? Number(r) < n.length : ie(n, r),
+        if (En(s) && Ae(s) && !Ae(o)) return !1;
+        if (!e && (!Rr(o) && !En(o) && (s = ee(s), o = ee(o)), !K(n) && Ae(s) && !Ae(o))) return s.value = o, !0;
+        const u = K(n) && gi(r) ? Number(r) < n.length : ie(n, r),
             c = Reflect.set(n, r, o, a);
-        return n === ee(a) && (u ? Yn(o, s) && Pt(n, "set", r, o) : Pt(n, "add", r, o)), c
+        return n === ee(a) && (u ? $n(o, s) && Pt(n, "set", r, o) : Pt(n, "add", r, o)), c
     }
 }
 
 function fm(e, t) {
     const n = ie(e, t);
     e[t];
     const r = Reflect.deleteProperty(e, t);
     return r && n && Pt(e, "delete", t, void 0), r
 }
 
 function _m(e, t) {
     const n = Reflect.has(e, t);
-    return (!gi(t) || !Sl.has(t)) && We(e, "has", t), n
+    return (!bi(t) || !Tl.has(t)) && We(e, "has", t), n
 }
 
 function pm(e) {
     return We(e, "iterate", K(e) ? "length" : Zt), Reflect.ownKeys(e)
 }
-const Pl = {
+const Al = {
         get: am,
         set: mm,
         deleteProperty: fm,
         has: _m,
         ownKeys: pm
     },
     hm = {
@@ -424,103 +424,103 @@
         set(e, t) {
             return !0
         },
         deleteProperty(e, t) {
             return !0
         }
     },
-    zm = ye({}, Pl, {
+    zm = ye({}, Al, {
         get: sm,
         set: dm
     }),
-    Ei = e => e,
-    Qr = e => Reflect.getPrototypeOf(e);
+    Pi = e => e,
+    Yr = e => Reflect.getPrototypeOf(e);
 
-function _r(e, t, n = !1, r = !1) {
+function fr(e, t, n = !1, r = !1) {
     e = e.__v_raw;
     const o = ee(e),
         a = ee(t);
     n || (t !== a && We(o, "get", t), We(o, "get", a));
     const {
         has: s
-    } = Qr(o), u = r ? Ei : n ? Ci : Qn;
+    } = Yr(o), u = r ? Pi : n ? wi : Yn;
     if (s.call(o, t)) return u(e.get(t));
     if (s.call(o, a)) return u(e.get(a));
     e !== o && e.get(t)
 }
 
-function pr(e, t = !1) {
+function _r(e, t = !1) {
     const n = this.__v_raw,
         r = ee(n),
         o = ee(e);
     return t || (e !== o && We(r, "has", e), We(r, "has", o)), e === o ? n.has(e) : n.has(e) || n.has(o)
 }
 
-function hr(e, t = !1) {
+function pr(e, t = !1) {
     return e = e.__v_raw, !t && We(ee(e), "iterate", Zt), Reflect.get(e, "size", e)
 }
 
-function fa(e) {
+function da(e) {
     e = ee(e);
     const t = ee(this);
-    return Qr(t).has.call(t, e) || (t.add(e), Pt(t, "add", e, e)), this
+    return Yr(t).has.call(t, e) || (t.add(e), Pt(t, "add", e, e)), this
 }
 
-function _a(e, t) {
+function fa(e, t) {
     t = ee(t);
     const n = ee(this),
         {
             has: r,
             get: o
-        } = Qr(n);
+        } = Yr(n);
     let a = r.call(n, e);
     a || (e = ee(e), a = r.call(n, e));
     const s = o.call(n, e);
-    return n.set(e, t), a ? Yn(t, s) && Pt(n, "set", e, t) : Pt(n, "add", e, t), this
+    return n.set(e, t), a ? $n(t, s) && Pt(n, "set", e, t) : Pt(n, "add", e, t), this
 }
 
-function pa(e) {
+function _a(e) {
     const t = ee(this),
         {
             has: n,
             get: r
-        } = Qr(t);
+        } = Yr(t);
     let o = n.call(t, e);
     o || (e = ee(e), o = n.call(t, e)), r && r.call(t, e);
     const a = t.delete(e);
     return o && Pt(t, "delete", e, void 0), a
 }
 
-function ha() {
+function pa() {
     const e = ee(this),
         t = e.size !== 0,
         n = e.clear();
     return t && Pt(e, "clear", void 0, void 0), n
 }
 
-function zr(e, t) {
+function hr(e, t) {
     return function(r, o) {
         const a = this,
             s = a.__v_raw,
             u = ee(s),
-            c = t ? Ei : e ? Ci : Qn;
+            c = t ? Pi : e ? wi : Yn;
         return !e && We(u, "iterate", Zt), s.forEach((l, d) => r.call(o, c(l), c(d), a))
     }
 }
 
-function br(e, t, n) {
+function zr(e, t, n) {
     return function(...r) {
         const o = this.__v_raw,
             a = ee(o),
-            s = Tn(a),
+            s = vn(a),
             u = e === "entries" || e === Symbol.iterator && s,
             c = e === "keys" && s,
             l = o[e](...r),
-            d = n ? Ei : t ? Ci : Qn;
-        return !t && We(a, "iterate", c ? Ho : Zt), {
+            d = n ? Pi : t ? wi : Yn;
+        return !t && We(a, "iterate", c ? No : Zt), {
             next() {
                 const {
                     value: m,
                     done: f
                 } = l.next();
                 return f ? {
                     value: m,
@@ -542,94 +542,94 @@
         return e === "delete" ? !1 : this
     }
 }
 
 function bm() {
     const e = {
             get(a) {
-                return _r(this, a)
+                return fr(this, a)
             },
             get size() {
-                return hr(this)
+                return pr(this)
             },
-            has: pr,
-            add: fa,
-            set: _a,
-            delete: pa,
-            clear: ha,
-            forEach: zr(!1, !1)
+            has: _r,
+            add: da,
+            set: fa,
+            delete: _a,
+            clear: pa,
+            forEach: hr(!1, !1)
         },
         t = {
             get(a) {
-                return _r(this, a, !1, !0)
+                return fr(this, a, !1, !0)
             },
             get size() {
-                return hr(this)
+                return pr(this)
             },
-            has: pr,
-            add: fa,
-            set: _a,
-            delete: pa,
-            clear: ha,
-            forEach: zr(!1, !0)
+            has: _r,
+            add: da,
+            set: fa,
+            delete: _a,
+            clear: pa,
+            forEach: hr(!1, !0)
         },
         n = {
             get(a) {
-                return _r(this, a, !0)
+                return fr(this, a, !0)
             },
             get size() {
-                return hr(this, !0)
+                return pr(this, !0)
             },
             has(a) {
-                return pr.call(this, a, !0)
+                return _r.call(this, a, !0)
             },
             add: wt("add"),
             set: wt("set"),
             delete: wt("delete"),
             clear: wt("clear"),
-            forEach: zr(!0, !1)
+            forEach: hr(!0, !1)
         },
         r = {
             get(a) {
-                return _r(this, a, !0, !0)
+                return fr(this, a, !0, !0)
             },
             get size() {
-                return hr(this, !0)
+                return pr(this, !0)
             },
             has(a) {
-                return pr.call(this, a, !0)
+                return _r.call(this, a, !0)
             },
             add: wt("add"),
             set: wt("set"),
             delete: wt("delete"),
             clear: wt("clear"),
-            forEach: zr(!0, !0)
+            forEach: hr(!0, !0)
         };
     return ["keys", "values", "entries", Symbol.iterator].forEach(a => {
-        e[a] = br(a, !1, !1), n[a] = br(a, !0, !1), t[a] = br(a, !1, !0), r[a] = br(a, !0, !0)
+        e[a] = zr(a, !1, !1), n[a] = zr(a, !0, !1), t[a] = zr(a, !1, !0), r[a] = zr(a, !0, !0)
     }), [e, n, t, r]
 }
 const [gm, ym, vm, Tm] = bm();
 
-function Mi(e, t) {
+function Ei(e, t) {
     const n = t ? e ? Tm : vm : e ? ym : gm;
     return (r, o, a) => o === "__v_isReactive" ? !e : o === "__v_isReadonly" ? e : o === "__v_raw" ? r : Reflect.get(ie(n, o) && o in r ? n : r, o, a)
 }
 const Sm = {
-        get: Mi(!1, !1)
+        get: Ei(!1, !1)
     },
     Am = {
-        get: Mi(!1, !0)
+        get: Ei(!1, !0)
     },
     Pm = {
-        get: Mi(!0, !1)
+        get: Ei(!0, !1)
     },
+    Pl = new WeakMap,
     El = new WeakMap,
     Ml = new WeakMap,
-    wl = new WeakMap,
     Em = new WeakMap;
 
 function Mm(e) {
     switch (e) {
         case "Object":
         case "Array":
             return 1;
@@ -644,118 +644,118 @@
 }
 
 function wm(e) {
     return e.__v_skip || !Object.isExtensible(e) ? 0 : Mm(Vu(e))
 }
 
 function Xe(e) {
-    return Mn(e) ? e : wi(e, !1, Pl, Sm, El)
+    return En(e) ? e : Mi(e, !1, Al, Sm, Pl)
 }
 
-function Cl(e) {
-    return wi(e, !1, zm, Am, Ml)
+function wl(e) {
+    return Mi(e, !1, zm, Am, El)
 }
 
-function kl(e) {
-    return wi(e, !0, hm, Pm, wl)
+function Cl(e) {
+    return Mi(e, !0, hm, Pm, Ml)
 }
 
-function wi(e, t, n, r, o) {
+function Mi(e, t, n, r, o) {
     if (!me(e) || e.__v_raw && !(t && e.__v_isReactive)) return e;
     const a = o.get(e);
     if (a) return a;
     const s = wm(e);
     if (s === 0) return e;
     const u = new Proxy(e, s === 2 ? r : n);
     return o.set(e, u), u
 }
 
-function Sn(e) {
-    return Mn(e) ? Sn(e.__v_raw) : !!(e && e.__v_isReactive)
+function Tn(e) {
+    return En(e) ? Tn(e.__v_raw) : !!(e && e.__v_isReactive)
 }
 
-function Mn(e) {
+function En(e) {
     return !!(e && e.__v_isReadonly)
 }
 
-function Lr(e) {
+function Rr(e) {
     return !!(e && e.__v_isShallow)
 }
 
-function Dl(e) {
-    return Sn(e) || Mn(e)
+function kl(e) {
+    return Tn(e) || En(e)
 }
 
 function ee(e) {
     const t = e && e.__v_raw;
     return t ? ee(t) : e
 }
 
-function Il(e) {
-    return Gr(e, "__v_skip", !0), e
+function Dl(e) {
+    return Or(e, "__v_skip", !0), e
 }
-const Qn = e => me(e) ? Xe(e) : e,
-    Ci = e => me(e) ? kl(e) : e;
+const Yn = e => me(e) ? Xe(e) : e,
+    wi = e => me(e) ? Cl(e) : e;
 
-function Ol(e) {
-    Gt && st && (e = ee(e), Tl(e.dep || (e.dep = Si())))
+function Il(e) {
+    Gt && st && (e = ee(e), vl(e.dep || (e.dep = Ti())))
 }
 
-function Gl(e, t) {
+function Ol(e, t) {
     e = ee(e);
     const n = e.dep;
-    n && xo(n)
+    n && Ho(n)
 }
 
 function Ae(e) {
     return !!(e && e.__v_isRef === !0)
 }
 
 function Me(e) {
-    return Rl(e, !1)
+    return Gl(e, !1)
 }
 
 function Jt(e) {
-    return Rl(e, !0)
+    return Gl(e, !0)
 }
 
-function Rl(e, t) {
+function Gl(e, t) {
     return Ae(e) ? e : new Cm(e, t)
 }
 class Cm {
     constructor(t, n) {
-        this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? t : ee(t), this._value = n ? t : Qn(t)
+        this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? t : ee(t), this._value = n ? t : Yn(t)
     }
     get value() {
-        return Ol(this), this._value
+        return Il(this), this._value
     }
     set value(t) {
-        const n = this.__v_isShallow || Lr(t) || Mn(t);
-        t = n ? t : ee(t), Yn(t, this._rawValue) && (this._rawValue = t, this._value = n ? t : Qn(t), Gl(this))
+        const n = this.__v_isShallow || Rr(t) || En(t);
+        t = n ? t : ee(t), $n(t, this._rawValue) && (this._rawValue = t, this._value = n ? t : Yn(t), Ol(this))
     }
 }
 
 function lt(e) {
     return Ae(e) ? e.value : e
 }
 const km = {
     get: (e, t, n) => lt(Reflect.get(e, t, n)),
     set: (e, t, n, r) => {
         const o = e[t];
         return Ae(o) && !Ae(n) ? (o.value = n, !0) : Reflect.set(e, t, n, r)
     }
 };
 
-function Ll(e) {
-    return Sn(e) ? e : new Proxy(e, km)
+function Rl(e) {
+    return Tn(e) ? e : new Proxy(e, km)
 }
 
-function ki(e) {
+function Ci(e) {
     const t = K(e) ? new Array(e.length) : {};
-    for (const n in e) t[n] = Bl(e, n);
+    for (const n in e) t[n] = Ll(e, n);
     return t
 }
 class Dm {
     constructor(t, n, r) {
         this._object = t, this._key = n, this._defaultValue = r, this.__v_isRef = !0
     }
     get value() {
@@ -775,30 +775,30 @@
     }
     get value() {
         return this._getter()
     }
 }
 
 function Kz(e, t, n) {
-    return Ae(e) ? e : Q(e) ? new Im(e) : me(e) && arguments.length > 1 ? Bl(e, t, n) : Me(e)
+    return Ae(e) ? e : Q(e) ? new Im(e) : me(e) && arguments.length > 1 ? Ll(e, t, n) : Me(e)
 }
 
-function Bl(e, t, n) {
+function Ll(e, t, n) {
     const r = e[t];
     return Ae(r) ? r : new Dm(e, t, n)
 }
 class Om {
     constructor(t, n, r, o) {
-        this._setter = n, this.dep = void 0, this.__v_isRef = !0, this.__v_isReadonly = !1, this._dirty = !0, this.effect = new Ai(t, () => {
-            this._dirty || (this._dirty = !0, Gl(this))
+        this._setter = n, this.dep = void 0, this.__v_isRef = !0, this.__v_isReadonly = !1, this._dirty = !0, this.effect = new Si(t, () => {
+            this._dirty || (this._dirty = !0, Ol(this))
         }), this.effect.computed = this, this.effect.active = this._cacheable = !o, this.__v_isReadonly = r
     }
     get value() {
         const t = ee(this);
-        return Ol(t), (t._dirty || !t._cacheable) && (t._dirty = !1, t._value = t.effect.run()), t._value
+        return Il(t), (t._dirty || !t._cacheable) && (t._dirty = !1, t._value = t.effect.run()), t._value
     }
     set value(t) {
         this._setter(t)
     }
 }
 
 function Gm(e, t, n = !1) {
@@ -808,32 +808,32 @@
 }
 
 function Rt(e, t, n, r) {
     let o;
     try {
         o = r ? e(...r) : e()
     } catch (a) {
-        Zr(a, t, n)
+        Qr(a, t, n)
     }
     return o
 }
 
 function tt(e, t, n, r) {
     if (Q(e)) {
         const a = Rt(e, t, n, r);
-        return a && dl(a) && a.catch(s => {
-            Zr(s, t, n)
+        return a && ml(a) && a.catch(s => {
+            Qr(s, t, n)
         }), a
     }
     const o = [];
     for (let a = 0; a < e.length; a++) o.push(tt(e[a], t, n, r));
     return o
 }
 
-function Zr(e, t, n, r = !0) {
+function Qr(e, t, n, r = !0) {
     const o = t ? t.vnode : null;
     if (t) {
         let a = t.parent;
         const s = t.proxy,
             u = n;
         for (; a;) {
             const l = a.ec;
@@ -851,94 +851,94 @@
     }
     Rm(e, n, o, r)
 }
 
 function Rm(e, t, n, r = !0) {
     console.error(e)
 }
-let Zn = !1,
-    Fo = !1;
+let Qn = !1,
+    xo = !1;
 const Le = [];
 let bt = 0;
-const An = [];
+const Sn = [];
 let St = null,
     Kt = 0;
-const Nl = Promise.resolve();
-let Di = null;
+const Bl = Promise.resolve();
+let ki = null;
 
-function Ii(e) {
-    const t = Di || Nl;
+function Di(e) {
+    const t = ki || Bl;
     return e ? t.then(this ? e.bind(this) : e) : t
 }
 
 function Lm(e) {
     let t = bt + 1,
         n = Le.length;
     for (; t < n;) {
         const r = t + n >>> 1;
-        Jn(Le[r]) < e ? t = r + 1 : n = r
+        Zn(Le[r]) < e ? t = r + 1 : n = r
     }
     return t
 }
 
-function Oi(e) {
-    (!Le.length || !Le.includes(e, Zn && e.allowRecurse ? bt + 1 : bt)) && (e.id == null ? Le.push(e) : Le.splice(Lm(e.id), 0, e), Hl())
+function Ii(e) {
+    (!Le.length || !Le.includes(e, Qn && e.allowRecurse ? bt + 1 : bt)) && (e.id == null ? Le.push(e) : Le.splice(Lm(e.id), 0, e), Nl())
 }
 
-function Hl() {
-    !Zn && !Fo && (Fo = !0, Di = Nl.then(Fl))
+function Nl() {
+    !Qn && !xo && (xo = !0, ki = Bl.then(xl))
 }
 
 function Bm(e) {
     const t = Le.indexOf(e);
     t > bt && Le.splice(t, 1)
 }
 
 function Nm(e) {
-    K(e) ? An.push(...e) : (!St || !St.includes(e, e.allowRecurse ? Kt + 1 : Kt)) && An.push(e), Hl()
+    K(e) ? Sn.push(...e) : (!St || !St.includes(e, e.allowRecurse ? Kt + 1 : Kt)) && Sn.push(e), Nl()
 }
 
-function za(e, t = Zn ? bt + 1 : 0) {
+function ha(e, t = Qn ? bt + 1 : 0) {
     for (; t < Le.length; t++) {
         const n = Le[t];
         n && n.pre && (Le.splice(t, 1), t--, n())
     }
 }
 
-function xl(e) {
-    if (An.length) {
-        const t = [...new Set(An)];
-        if (An.length = 0, St) {
+function Hl(e) {
+    if (Sn.length) {
+        const t = [...new Set(Sn)];
+        if (Sn.length = 0, St) {
             St.push(...t);
             return
         }
-        for (St = t, St.sort((n, r) => Jn(n) - Jn(r)), Kt = 0; Kt < St.length; Kt++) St[Kt]();
+        for (St = t, St.sort((n, r) => Zn(n) - Zn(r)), Kt = 0; Kt < St.length; Kt++) St[Kt]();
         St = null, Kt = 0
     }
 }
-const Jn = e => e.id == null ? 1 / 0 : e.id,
+const Zn = e => e.id == null ? 1 / 0 : e.id,
     Hm = (e, t) => {
-        const n = Jn(e) - Jn(t);
+        const n = Zn(e) - Zn(t);
         if (n === 0) {
             if (e.pre && !t.pre) return -1;
             if (t.pre && !e.pre) return 1
         }
         return n
     };
 
-function Fl(e) {
-    Fo = !1, Zn = !0, Le.sort(Hm);
+function xl(e) {
+    xo = !1, Qn = !0, Le.sort(Hm);
     const t = mt;
     try {
         for (bt = 0; bt < Le.length; bt++) {
             const n = Le[bt];
             n && n.active !== !1 && Rt(n, null, 14)
         }
     } finally {
-        bt = 0, Le.length = 0, xl(), Zn = !1, Di = null, (Le.length || An.length) && Fl()
+        bt = 0, Le.length = 0, Hl(), Qn = !1, ki = null, (Le.length || Sn.length) && xl()
     }
 }
 
 function xm(e, t, ...n) {
     if (e.isUnmounted) return;
     const r = e.vnode.props || de;
     let o = n;
@@ -948,78 +948,78 @@
         const d = `${s==="modelValue"?"model":s}Modifiers`,
             {
                 number: m,
                 trim: f
             } = r[d] || de;
         f && (o = n.map(_ => be(_) ? _.trim() : _)), m && (o = n.map(ju))
     }
-    let u, c = r[u = Dr(t)] || r[u = Dr(gt(t))];
-    !c && a && (c = r[u = Dr(nn(t))]), c && tt(c, e, 6, o);
+    let u, c = r[u = kr(t)] || r[u = kr(gt(t))];
+    !c && a && (c = r[u = kr(nn(t))]), c && tt(c, e, 6, o);
     const l = r[u + "Once"];
     if (l) {
         if (!e.emitted) e.emitted = {};
         else if (e.emitted[u]) return;
         e.emitted[u] = !0, tt(l, e, 6, o)
     }
 }
 
-function Vl(e, t, n = !1) {
+function Fl(e, t, n = !1) {
     const r = t.emitsCache,
         o = r.get(e);
     if (o !== void 0) return o;
     const a = e.emits;
     let s = {},
         u = !1;
     if (!Q(e)) {
         const c = l => {
-            const d = Vl(l, t, !0);
+            const d = Fl(l, t, !0);
             d && (u = !0, ye(s, d))
         };
         !n && t.mixins.length && t.mixins.forEach(c), e.extends && c(e.extends), e.mixins && e.mixins.forEach(c)
     }
     return !a && !u ? (me(e) && r.set(e, null), null) : (K(a) ? a.forEach(c => s[c] = null) : ye(s, a), me(e) && r.set(e, s), s)
 }
 
-function Jr(e, t) {
-    return !e || !Xr(t) ? !1 : (t = t.slice(2).replace(/Once$/, ""), ie(e, t[0].toLowerCase() + t.slice(1)) || ie(e, nn(t)) || ie(e, t))
+function Zr(e, t) {
+    return !e || !Kr(t) ? !1 : (t = t.slice(2).replace(/Once$/, ""), ie(e, t[0].toLowerCase() + t.slice(1)) || ie(e, nn(t)) || ie(e, t))
 }
 let Oe = null,
-    eo = null;
+    Jr = null;
 
-function Br(e) {
+function Lr(e) {
     const t = Oe;
-    return Oe = e, eo = e && e.type.__scopeId || null, t
+    return Oe = e, Jr = e && e.type.__scopeId || null, t
 }
 
 function Xz(e) {
-    eo = e
+    Jr = e
 }
 
 function $z() {
-    eo = null
+    Jr = null
 }
-const Yz = e => Ul;
+const Yz = e => Vl;
 
-function Ul(e, t = Oe, n) {
+function Vl(e, t = Oe, n) {
     if (!t || e._n) return e;
     const r = (...o) => {
-        r._d && ka(-1);
-        const a = Br(t);
+        r._d && Ca(-1);
+        const a = Lr(t);
         let s;
         try {
             s = e(...o)
         } finally {
-            Br(a), r._d && ka(1)
+            Lr(a), r._d && Ca(1)
         }
         return s
     };
     return r._n = !0, r._c = !0, r._d = !0, r
 }
 
-function vo(e) {
+function yo(e) {
     const {
         type: t,
         vnode: n,
         proxy: r,
         withProxy: o,
         props: a,
         propsOptions: [s],
@@ -1030,48 +1030,48 @@
         renderCache: m,
         data: f,
         setupState: _,
         ctx: p,
         inheritAttrs: b
     } = e;
     let T, v;
-    const A = Br(e);
+    const A = Lr(e);
     try {
         if (n.shapeFlag & 4) {
             const P = o || r;
             T = ht(d.call(P, P, m, a, _, f, p)), v = c
         } else {
             const P = t;
             T = ht(P.length > 1 ? P(a, {
                 attrs: c,
                 slots: u,
                 emit: l
             }) : P(a, null)), v = t.props ? c : Fm(c)
         }
     } catch (P) {
-        jn.length = 0, Zr(P, e, 1), T = fe(nt)
+        Wn.length = 0, Qr(P, e, 1), T = fe(nt)
     }
     let I = T;
     if (v && b !== !1) {
         const P = Object.keys(v),
             {
                 shapeFlag: M
             } = I;
-        P.length && M & 7 && (s && P.some(zi) && (v = Vm(v, s)), I = Nt(I, v))
+        P.length && M & 7 && (s && P.some(hi) && (v = Vm(v, s)), I = Nt(I, v))
     }
-    return n.dirs && (I = Nt(I), I.dirs = I.dirs ? I.dirs.concat(n.dirs) : n.dirs), n.transition && (I.transition = n.transition), T = I, Br(A), T
+    return n.dirs && (I = Nt(I), I.dirs = I.dirs ? I.dirs.concat(n.dirs) : n.dirs), n.transition && (I.transition = n.transition), T = I, Lr(A), T
 }
 const Fm = e => {
         let t;
-        for (const n in e)(n === "class" || n === "style" || Xr(n)) && ((t || (t = {}))[n] = e[n]);
+        for (const n in e)(n === "class" || n === "style" || Kr(n)) && ((t || (t = {}))[n] = e[n]);
         return t
     },
     Vm = (e, t) => {
         const n = {};
-        for (const r in e)(!zi(r) || !(r.slice(9) in t)) && (n[r] = e[r]);
+        for (const r in e)(!hi(r) || !(r.slice(9) in t)) && (n[r] = e[r]);
         return n
     };
 
 function Um(e, t, n) {
     const {
         props: r,
         children: o,
@@ -1080,32 +1080,32 @@
         props: s,
         children: u,
         patchFlag: c
     } = t, l = a.emitsOptions;
     if (t.dirs || t.transition) return !0;
     if (n && c >= 0) {
         if (c & 1024) return !0;
-        if (c & 16) return r ? ba(r, s, l) : !!s;
+        if (c & 16) return r ? za(r, s, l) : !!s;
         if (c & 8) {
             const d = t.dynamicProps;
             for (let m = 0; m < d.length; m++) {
                 const f = d[m];
-                if (s[f] !== r[f] && !Jr(l, f)) return !0
+                if (s[f] !== r[f] && !Zr(l, f)) return !0
             }
         }
-    } else return (o || u) && (!u || !u.$stable) ? !0 : r === s ? !1 : r ? s ? ba(r, s, l) : !0 : !!s;
+    } else return (o || u) && (!u || !u.$stable) ? !0 : r === s ? !1 : r ? s ? za(r, s, l) : !0 : !!s;
     return !1
 }
 
-function ba(e, t, n) {
+function za(e, t, n) {
     const r = Object.keys(t);
     if (r.length !== Object.keys(e).length) return !0;
     for (let o = 0; o < r.length; o++) {
         const a = r[o];
-        if (t[a] !== e[a] && !Jr(n, a)) return !0
+        if (t[a] !== e[a] && !Zr(n, a)) return !0
     }
     return !1
 }
 
 function Wm({
     vnode: e,
     parent: t
@@ -1114,111 +1114,111 @@
 }
 const jm = e => e.__isSuspense;
 
 function qm(e, t) {
     t && t.pendingBranch ? K(e) ? t.effects.push(...e) : t.effects.push(e) : Nm(e)
 }
 
-function to(e, t) {
-    return Gi(e, null, t)
+function eo(e, t) {
+    return Oi(e, null, t)
 }
-const gr = {};
+const br = {};
 
 function xe(e, t, n) {
-    return Gi(e, t, n)
+    return Oi(e, t, n)
 }
 
-function Gi(e, t, {
+function Oi(e, t, {
     immediate: n,
     deep: r,
     flush: o,
     onTrack: a,
     onTrigger: s
 } = de) {
     var u;
     const c = em() === ((u = we) == null ? void 0 : u.scope) ? we : null;
     let l, d = !1,
         m = !1;
-    if (Ae(e) ? (l = () => e.value, d = Lr(e)) : Sn(e) ? (l = () => e, r = !0) : K(e) ? (m = !0, d = e.some(P => Sn(P) || Lr(P)), l = () => e.map(P => {
+    if (Ae(e) ? (l = () => e.value, d = Rr(e)) : Tn(e) ? (l = () => e, r = !0) : K(e) ? (m = !0, d = e.some(P => Tn(P) || Rr(P)), l = () => e.map(P => {
             if (Ae(P)) return P.value;
-            if (Sn(P)) return Yt(P);
+            if (Tn(P)) return Yt(P);
             if (Q(P)) return Rt(P, c, 2)
         })) : Q(e) ? t ? l = () => Rt(e, c, 2) : l = () => {
             if (!(c && c.isUnmounted)) return f && f(), tt(e, c, 3, [_])
         } : l = mt, t && r) {
         const P = l;
         l = () => Yt(P())
     }
     let f, _ = P => {
             f = A.onStop = () => {
                 Rt(P, c, 4)
             }
         },
         p;
-    if (rr)
+    if (nr)
         if (_ = mt, t ? n && tt(t, c, 3, [l(), m ? [] : void 0, _]) : l(), o === "sync") {
             const P = xd();
             p = P.__watcherHandles || (P.__watcherHandles = [])
         } else return mt;
-    let b = m ? new Array(e.length).fill(gr) : gr;
+    let b = m ? new Array(e.length).fill(br) : br;
     const T = () => {
         if (A.active)
             if (t) {
                 const P = A.run();
-                (r || d || (m ? P.some((M, N) => Yn(M, b[N])) : Yn(P, b))) && (f && f(), tt(t, c, 3, [P, b === gr ? void 0 : m && b[0] === gr ? [] : b, _]), b = P)
+                (r || d || (m ? P.some((M, N) => $n(M, b[N])) : $n(P, b))) && (f && f(), tt(t, c, 3, [P, b === br ? void 0 : m && b[0] === br ? [] : b, _]), b = P)
             } else A.run()
     };
     T.allowRecurse = !!t;
     let v;
-    o === "sync" ? v = T : o === "post" ? v = () => Ue(T, c && c.suspense) : (T.pre = !0, c && (T.id = c.uid), v = () => Oi(T));
-    const A = new Ai(l, v);
+    o === "sync" ? v = T : o === "post" ? v = () => Ue(T, c && c.suspense) : (T.pre = !0, c && (T.id = c.uid), v = () => Ii(T));
+    const A = new Si(l, v);
     t ? n ? T() : b = A.run() : o === "post" ? Ue(A.run.bind(A), c && c.suspense) : A.run();
     const I = () => {
-        A.stop(), c && c.scope && bi(c.scope.effects, A)
+        A.stop(), c && c.scope && zi(c.scope.effects, A)
     };
     return p && p.push(I), I
 }
 
 function Km(e, t, n) {
     const r = this.proxy,
-        o = be(e) ? e.includes(".") ? Wl(r, e) : () => r[e] : e.bind(r, r);
+        o = be(e) ? e.includes(".") ? Ul(r, e) : () => r[e] : e.bind(r, r);
     let a;
     Q(t) ? a = t : (a = t.handler, n = t);
     const s = we;
-    wn(this);
-    const u = Gi(o, a.bind(r), n);
-    return s ? wn(s) : en(), u
+    Mn(this);
+    const u = Oi(o, a.bind(r), n);
+    return s ? Mn(s) : en(), u
 }
 
-function Wl(e, t) {
+function Ul(e, t) {
     const n = t.split(".");
     return () => {
         let r = e;
         for (let o = 0; o < n.length && r; o++) r = r[n[o]];
         return r
     }
 }
 
 function Yt(e, t) {
     if (!me(e) || e.__v_skip || (t = t || new Set, t.has(e))) return e;
     if (t.add(e), Ae(e)) Yt(e.value, t);
     else if (K(e))
         for (let n = 0; n < e.length; n++) Yt(e[n], t);
-    else if (ml(e) || Tn(e)) e.forEach(n => {
+    else if (ul(e) || vn(e)) e.forEach(n => {
         Yt(n, t)
     });
-    else if (_l(e))
+    else if (fl(e))
         for (const n in e) Yt(e[n], t);
     return e
 }
 
 function Qz(e, t) {
     const n = Oe;
     if (n === null) return e;
-    const r = so(n) || n.proxy,
+    const r = ao(n) || n.proxy,
         o = e.dirs || (e.dirs = []);
     for (let a = 0; a < t.length; a++) {
         let [s, u, c, l = de] = t[a];
         s && (Q(s) && (s = {
             mounted: s,
             updated: s
         }), s.deep && Yt(u), o.push({
@@ -1236,33 +1236,33 @@
 function Vt(e, t, n, r) {
     const o = e.dirs,
         a = t && t.dirs;
     for (let s = 0; s < o.length; s++) {
         const u = o[s];
         a && (u.oldValue = a[s].value);
         let c = u.dir[r];
-        c && (Dn(), tt(c, n, 8, [e.el, u, e, t]), In())
+        c && (kn(), tt(c, n, 8, [e.el, u, e, t]), Dn())
     }
 }
 
-function jl() {
+function Wl() {
     const e = {
         isMounted: !1,
         isLeaving: !1,
         isUnmounting: !1,
         leavingVNodes: new Map
     };
-    return io(() => {
+    return oo(() => {
         e.isMounted = !0
-    }), Yl(() => {
+    }), $l(() => {
         e.isUnmounting = !0
     }), e
 }
 const Je = [Function, Array],
-    ql = {
+    jl = {
         mode: String,
         appear: Boolean,
         persisted: Boolean,
         onBeforeEnter: Je,
         onEnter: Je,
         onAfterEnter: Je,
         onEnterCancelled: Je,
@@ -1273,78 +1273,78 @@
         onBeforeAppear: Je,
         onAppear: Je,
         onAfterAppear: Je,
         onAppearCancelled: Je
     },
     Xm = {
         name: "BaseTransition",
-        props: ql,
+        props: jl,
         setup(e, {
             slots: t
         }) {
-            const n = On(),
-                r = jl();
+            const n = In(),
+                r = Wl();
             let o;
             return () => {
-                const a = t.default && Ri(t.default(), !0);
+                const a = t.default && Gi(t.default(), !0);
                 if (!a || !a.length) return;
                 let s = a[0];
                 if (a.length > 1) {
                     for (const b of a)
                         if (b.type !== nt) {
                             s = b;
                             break
                         }
                 }
                 const u = ee(e),
                     {
                         mode: c
                     } = u;
-                if (r.isLeaving) return To(s);
-                const l = ga(s);
-                if (!l) return To(s);
-                const d = er(l, u, r, n);
-                tr(l, d);
+                if (r.isLeaving) return vo(s);
+                const l = ba(s);
+                if (!l) return vo(s);
+                const d = Jn(l, u, r, n);
+                er(l, d);
                 const m = n.subTree,
-                    f = m && ga(m);
+                    f = m && ba(m);
                 let _ = !1;
                 const {
                     getTransitionKey: p
                 } = l.type;
                 if (p) {
                     const b = p();
                     o === void 0 ? o = b : b !== o && (o = b, _ = !0)
                 }
                 if (f && f.type !== nt && (!Xt(l, f) || _)) {
-                    const b = er(f, u, r, n);
-                    if (tr(f, b), c === "out-in") return r.isLeaving = !0, b.afterLeave = () => {
+                    const b = Jn(f, u, r, n);
+                    if (er(f, b), c === "out-in") return r.isLeaving = !0, b.afterLeave = () => {
                         r.isLeaving = !1, n.update.active !== !1 && n.update()
-                    }, To(s);
+                    }, vo(s);
                     c === "in-out" && l.type !== nt && (b.delayLeave = (T, v, A) => {
-                        const I = Kl(r, f);
+                        const I = ql(r, f);
                         I[String(f.key)] = f, T._leaveCb = () => {
                             v(), T._leaveCb = void 0, delete d.delayedLeave
                         }, d.delayedLeave = A
                     })
                 }
                 return s
             }
         }
     },
     $m = Xm;
 
-function Kl(e, t) {
+function ql(e, t) {
     const {
         leavingVNodes: n
     } = e;
     let r = n.get(t.type);
     return r || (r = Object.create(null), n.set(t.type, r)), r
 }
 
-function er(e, t, n, r) {
+function Jn(e, t, n, r) {
     const {
         appear: o,
         mode: a,
         persisted: s = !1,
         onBeforeEnter: u,
         onEnter: c,
         onAfterEnter: l,
@@ -1353,15 +1353,15 @@
         onLeave: f,
         onAfterLeave: _,
         onLeaveCancelled: p,
         onBeforeAppear: b,
         onAppear: T,
         onAfterAppear: v,
         onAppearCancelled: A
-    } = t, I = String(e.key), P = Kl(n, e), M = (L, X) => {
+    } = t, I = String(e.key), P = ql(n, e), M = (L, X) => {
         L && tt(L, r, 9, X)
     }, N = (L, X) => {
         const $ = X[1];
         M(L, X), K(L) ? L.every(Y => Y.length <= 1) && $() : L.length <= 1 && $()
     }, j = {
         mode: a,
         persisted: s,
@@ -1394,144 +1394,144 @@
             let Y = !1;
             const x = L._leaveCb = te => {
                 Y || (Y = !0, X(), te ? M(p, [L]) : M(_, [L]), L._leaveCb = void 0, P[$] === e && delete P[$])
             };
             P[$] = e, f ? N(f, [L, x]) : x()
         },
         clone(L) {
-            return er(L, t, n, r)
+            return Jn(L, t, n, r)
         }
     };
     return j
 }
 
-function To(e) {
-    if (ro(e)) return e = Nt(e), e.children = null, e
+function vo(e) {
+    if (no(e)) return e = Nt(e), e.children = null, e
 }
 
-function ga(e) {
-    return ro(e) ? e.children ? e.children[0] : void 0 : e
+function ba(e) {
+    return no(e) ? e.children ? e.children[0] : void 0 : e
 }
 
-function tr(e, t) {
-    e.shapeFlag & 6 && e.component ? tr(e.component.subTree, t) : e.shapeFlag & 128 ? (e.ssContent.transition = t.clone(e.ssContent), e.ssFallback.transition = t.clone(e.ssFallback)) : e.transition = t
+function er(e, t) {
+    e.shapeFlag & 6 && e.component ? er(e.component.subTree, t) : e.shapeFlag & 128 ? (e.ssContent.transition = t.clone(e.ssContent), e.ssFallback.transition = t.clone(e.ssFallback)) : e.transition = t
 }
 
-function Ri(e, t = !1, n) {
+function Gi(e, t = !1, n) {
     let r = [],
         o = 0;
     for (let a = 0; a < e.length; a++) {
         let s = e[a];
         const u = n == null ? s.key : String(n) + String(s.key != null ? s.key : a);
-        s.type === He ? (s.patchFlag & 128 && o++, r = r.concat(Ri(s.children, t, u))) : (t || s.type !== nt) && r.push(u != null ? Nt(s, {
+        s.type === He ? (s.patchFlag & 128 && o++, r = r.concat(Gi(s.children, t, u))) : (t || s.type !== nt) && r.push(u != null ? Nt(s, {
             key: u
         }) : s)
     }
     if (o > 1)
         for (let a = 0; a < r.length; a++) r[a].patchFlag = -2;
     return r
 }
 
-function no(e, t) {
+function to(e, t) {
     return Q(e) ? (() => ye({
         name: e.name
     }, t, {
         setup: e
     }))() : e
 }
-const Vn = e => !!e.type.__asyncLoader,
-    ro = e => e.type.__isKeepAlive;
+const Fn = e => !!e.type.__asyncLoader,
+    no = e => e.type.__isKeepAlive;
 
 function Ym(e, t) {
-    Xl(e, "a", t)
+    Kl(e, "a", t)
 }
 
 function Qm(e, t) {
-    Xl(e, "da", t)
+    Kl(e, "da", t)
 }
 
-function Xl(e, t, n = we) {
+function Kl(e, t, n = we) {
     const r = e.__wdc || (e.__wdc = () => {
         let o = n;
         for (; o;) {
             if (o.isDeactivated) return;
             o = o.parent
         }
         return e()
     });
-    if (oo(t, r, n), n) {
+    if (ro(t, r, n), n) {
         let o = n.parent;
-        for (; o && o.parent;) ro(o.parent.vnode) && Zm(r, t, n, o), o = o.parent
+        for (; o && o.parent;) no(o.parent.vnode) && Zm(r, t, n, o), o = o.parent
     }
 }
 
 function Zm(e, t, n, r) {
-    const o = oo(t, e, r, !0);
-    Li(() => {
-        bi(r[t], o)
+    const o = ro(t, e, r, !0);
+    Ri(() => {
+        zi(r[t], o)
     }, n)
 }
 
-function oo(e, t, n = we, r = !1) {
+function ro(e, t, n = we, r = !1) {
     if (n) {
         const o = n[e] || (n[e] = []),
             a = t.__weh || (t.__weh = (...s) => {
                 if (n.isUnmounted) return;
-                Dn(), wn(n);
+                kn(), Mn(n);
                 const u = tt(t, n, e, s);
-                return en(), In(), u
+                return en(), Dn(), u
             });
         return r ? o.unshift(a) : o.push(a), a
     }
 }
-const Et = e => (t, n = we) => (!rr || e === "sp") && oo(e, (...r) => t(...r), n),
+const Et = e => (t, n = we) => (!nr || e === "sp") && ro(e, (...r) => t(...r), n),
     Jm = Et("bm"),
-    io = Et("m"),
+    oo = Et("m"),
     ed = Et("bu"),
-    $l = Et("u"),
-    Yl = Et("bum"),
-    Li = Et("um"),
+    Xl = Et("u"),
+    $l = Et("bum"),
+    Ri = Et("um"),
     td = Et("sp"),
     nd = Et("rtg"),
     rd = Et("rtc");
 
 function od(e, t = we) {
-    oo("ec", e, t)
+    ro("ec", e, t)
 }
-const Bi = "components",
+const Li = "components",
     id = "directives";
 
 function ad(e, t) {
-    return Ni(Bi, e, !0, t) || e
+    return Bi(Li, e, !0, t) || e
 }
-const Ql = Symbol.for("v-ndc");
+const Yl = Symbol.for("v-ndc");
 
 function Zz(e) {
-    return be(e) ? Ni(Bi, e, !1) || e : e || Ql
+    return be(e) ? Bi(Li, e, !1) || e : e || Yl
 }
 
 function Jz(e) {
-    return Ni(id, e)
+    return Bi(id, e)
 }
 
-function Ni(e, t, n = !0, r = !1) {
+function Bi(e, t, n = !0, r = !1) {
     const o = Oe || we;
     if (o) {
         const a = o.type;
-        if (e === Bi) {
+        if (e === Li) {
             const u = Bd(a, !1);
-            if (u && (u === t || u === gt(t) || u === ur(gt(t)))) return a
+            if (u && (u === t || u === gt(t) || u === cr(gt(t)))) return a
         }
-        const s = ya(o[e] || a[e], t) || ya(o.appContext[e], t);
+        const s = ga(o[e] || a[e], t) || ga(o.appContext[e], t);
         return !s && r ? a : s
     }
 }
 
-function ya(e, t) {
-    return e && (e[t] || e[gt(t)] || e[ur(gt(t))])
+function ga(e, t) {
+    return e && (e[t] || e[gt(t)] || e[cr(gt(t))])
 }
 
 function eb(e, t, n, r) {
     let o;
     const a = n && n[r];
     if (K(e) || be(e)) {
         o = new Array(e.length);
@@ -1563,51 +1563,51 @@
             return a && (a.key = r.key), a
         } : r.fn)
     }
     return e
 }
 
 function nb(e, t, n = {}, r, o) {
-    if (Oe.isCE || Oe.parent && Vn(Oe.parent) && Oe.parent.isCE) return t !== "default" && (n.name = t), fe("slot", n, r && r());
+    if (Oe.isCE || Oe.parent && Fn(Oe.parent) && Oe.parent.isCE) return t !== "default" && (n.name = t), fe("slot", n, r && r());
     let a = e[t];
-    a && a._c && (a._d = !1), Vi();
-    const s = a && Zl(a(n)),
-        u = Ui(He, {
+    a && a._c && (a._d = !1), Fi();
+    const s = a && Ql(a(n)),
+        u = Vi(He, {
             key: n.key || s && s.key || `_${t}`
         }, s || (r ? r() : []), s && e._ === 1 ? 64 : -2);
     return !o && u.scopeId && (u.slotScopeIds = [u.scopeId + "-s"]), a && a._c && (a._d = !0), u
 }
 
-function Zl(e) {
-    return e.some(t => xr(t) ? !(t.type === nt || t.type === He && !Zl(t.children)) : !0) ? e : null
+function Ql(e) {
+    return e.some(t => Hr(t) ? !(t.type === nt || t.type === He && !Ql(t.children)) : !0) ? e : null
 }
 
 function rb(e, t) {
     const n = {};
-    for (const r in e) n[t && /[A-Z]/.test(r) ? `on:${r}` : Dr(r)] = e[r];
+    for (const r in e) n[t && /[A-Z]/.test(r) ? `on:${r}` : kr(r)] = e[r];
     return n
 }
-const Vo = e => e ? mc(e) ? so(e) || e.proxy : Vo(e.parent) : null,
-    Un = ye(Object.create(null), {
+const Fo = e => e ? uc(e) ? ao(e) || e.proxy : Fo(e.parent) : null,
+    Vn = ye(Object.create(null), {
         $: e => e,
         $el: e => e.vnode.el,
         $data: e => e.data,
         $props: e => e.props,
         $attrs: e => e.attrs,
         $slots: e => e.slots,
         $refs: e => e.refs,
-        $parent: e => Vo(e.parent),
-        $root: e => Vo(e.root),
+        $parent: e => Fo(e.parent),
+        $root: e => Fo(e.root),
         $emit: e => e.emit,
-        $options: e => Hi(e),
-        $forceUpdate: e => e.f || (e.f = () => Oi(e.update)),
-        $nextTick: e => e.n || (e.n = Ii.bind(e.proxy)),
+        $options: e => Ni(e),
+        $forceUpdate: e => e.f || (e.f = () => Ii(e.update)),
+        $nextTick: e => e.n || (e.n = Di.bind(e.proxy)),
         $watch: e => Km.bind(e)
     }),
-    So = (e, t) => e !== de && !e.__isScriptSetup && ie(e, t),
+    To = (e, t) => e !== de && !e.__isScriptSetup && ie(e, t),
     sd = {
         get({
             _: e
         }, t) {
             const {
                 ctx: n,
                 setupState: r,
@@ -1626,66 +1626,66 @@
                     case 2:
                         return o[t];
                     case 4:
                         return n[t];
                     case 3:
                         return a[t]
                 } else {
-                    if (So(r, t)) return s[t] = 1, r[t];
+                    if (To(r, t)) return s[t] = 1, r[t];
                     if (o !== de && ie(o, t)) return s[t] = 2, o[t];
                     if ((l = e.propsOptions[0]) && ie(l, t)) return s[t] = 3, a[t];
                     if (n !== de && ie(n, t)) return s[t] = 4, n[t];
-                    Uo && (s[t] = 0)
+                    Vo && (s[t] = 0)
                 }
             }
-            const d = Un[t];
+            const d = Vn[t];
             let m, f;
             if (d) return t === "$attrs" && We(e, "get", t), d(e);
             if ((m = u.__cssModules) && (m = m[t])) return m;
             if (n !== de && ie(n, t)) return s[t] = 4, n[t];
             if (f = c.config.globalProperties, ie(f, t)) return f[t]
         },
         set({
             _: e
         }, t, n) {
             const {
                 data: r,
                 setupState: o,
                 ctx: a
             } = e;
-            return So(o, t) ? (o[t] = n, !0) : r !== de && ie(r, t) ? (r[t] = n, !0) : ie(e.props, t) || t[0] === "$" && t.slice(1) in e ? !1 : (a[t] = n, !0)
+            return To(o, t) ? (o[t] = n, !0) : r !== de && ie(r, t) ? (r[t] = n, !0) : ie(e.props, t) || t[0] === "$" && t.slice(1) in e ? !1 : (a[t] = n, !0)
         },
         has({
             _: {
                 data: e,
                 setupState: t,
                 accessCache: n,
                 ctx: r,
                 appContext: o,
                 propsOptions: a
             }
         }, s) {
             let u;
-            return !!n[s] || e !== de && ie(e, s) || So(t, s) || (u = a[0]) && ie(u, s) || ie(r, s) || ie(Un, s) || ie(o.config.globalProperties, s)
+            return !!n[s] || e !== de && ie(e, s) || To(t, s) || (u = a[0]) && ie(u, s) || ie(r, s) || ie(Vn, s) || ie(o.config.globalProperties, s)
         },
         defineProperty(e, t, n) {
             return n.get != null ? e._.accessCache[t] = 0 : ie(n, "value") && this.set(e, t, n.value, null), Reflect.defineProperty(e, t, n)
         }
     };
 
-function va(e) {
+function ya(e) {
     return K(e) ? e.reduce((t, n) => (t[n] = null, t), {}) : e
 }
-let Uo = !0;
+let Vo = !0;
 
 function ld(e) {
-    const t = Hi(e),
+    const t = Ni(e),
         n = e.proxy,
         r = e.ctx;
-    Uo = !1, t.beforeCreate && Ta(t.beforeCreate, e, "bc");
+    Vo = !1, t.beforeCreate && va(t.beforeCreate, e, "bc");
     const {
         data: o,
         computed: a,
         methods: s,
         watch: u,
         provide: c,
         inject: l,
@@ -1716,15 +1716,15 @@
             const oe = s[ne];
             Q(oe) && (r[ne] = oe.bind(n))
         }
     if (o) {
         const ne = o.call(n, n);
         me(ne) && (e.data = Xe(ne))
     }
-    if (Uo = !0, a)
+    if (Vo = !0, a)
         for (const ne in a) {
             const oe = a[ne],
                 it = Q(oe) ? oe.bind(n, n) : Q(oe.get) ? oe.get.bind(n, n) : mt,
                 ft = !Q(oe) && Q(oe.set) ? oe.set.bind(n) : mt,
                 Qe = re({
                     get: it,
                     set: ft
@@ -1733,168 +1733,168 @@
                 enumerable: !0,
                 configurable: !0,
                 get: () => Qe.value,
                 set: Ge => Qe.value = Ge
             })
         }
     if (u)
-        for (const ne in u) Jl(u[ne], r, n, ne);
+        for (const ne in u) Zl(u[ne], r, n, ne);
     if (c) {
         const ne = Q(c) ? c.call(n) : c;
         Reflect.ownKeys(ne).forEach(oe => {
-            Pn(oe, ne[oe])
+            An(oe, ne[oe])
         })
     }
-    d && Ta(d, e, "c");
+    d && va(d, e, "c");
 
     function _e(ne, oe) {
         K(oe) ? oe.forEach(it => ne(it.bind(n))) : oe && ne(oe.bind(n))
     }
-    if (_e(Jm, m), _e(io, f), _e(ed, _), _e($l, p), _e(Ym, b), _e(Qm, T), _e(od, L), _e(rd, N), _e(nd, j), _e(Yl, A), _e(Li, P), _e(td, X), K($))
+    if (_e(Jm, m), _e(oo, f), _e(ed, _), _e(Xl, p), _e(Ym, b), _e(Qm, T), _e(od, L), _e(rd, N), _e(nd, j), _e($l, A), _e(Ri, P), _e(td, X), K($))
         if ($.length) {
             const ne = e.exposed || (e.exposed = {});
             $.forEach(oe => {
                 Object.defineProperty(ne, oe, {
                     get: () => n[oe],
                     set: it => n[oe] = it
                 })
             })
         } else e.exposed || (e.exposed = {});
     M && e.render === mt && (e.render = M), Y != null && (e.inheritAttrs = Y), x && (e.components = x), te && (e.directives = te)
 }
 
 function cd(e, t, n = mt) {
-    K(e) && (e = Wo(e));
+    K(e) && (e = Uo(e));
     for (const r in e) {
         const o = e[r];
         let a;
         me(o) ? "default" in o ? a = ke(o.from || r, o.default, !0) : a = ke(o.from || r) : a = ke(o), Ae(a) ? Object.defineProperty(t, r, {
             enumerable: !0,
             configurable: !0,
             get: () => a.value,
             set: s => a.value = s
         }) : t[r] = a
     }
 }
 
-function Ta(e, t, n) {
+function va(e, t, n) {
     tt(K(e) ? e.map(r => r.bind(t.proxy)) : e.bind(t.proxy), t, n)
 }
 
-function Jl(e, t, n, r) {
-    const o = r.includes(".") ? Wl(n, r) : () => n[r];
+function Zl(e, t, n, r) {
+    const o = r.includes(".") ? Ul(n, r) : () => n[r];
     if (be(e)) {
         const a = t[e];
         Q(a) && xe(o, a)
     } else if (Q(e)) xe(o, e.bind(n));
     else if (me(e))
-        if (K(e)) e.forEach(a => Jl(a, t, n, r));
+        if (K(e)) e.forEach(a => Zl(a, t, n, r));
         else {
             const a = Q(e.handler) ? e.handler.bind(n) : t[e.handler];
             Q(a) && xe(o, a, e)
         }
 }
 
-function Hi(e) {
+function Ni(e) {
     const t = e.type,
         {
             mixins: n,
             extends: r
         } = t,
         {
             mixins: o,
             optionsCache: a,
             config: {
                 optionMergeStrategies: s
             }
         } = e.appContext,
         u = a.get(t);
     let c;
-    return u ? c = u : !o.length && !n && !r ? c = t : (c = {}, o.length && o.forEach(l => Nr(c, l, s, !0)), Nr(c, t, s)), me(t) && a.set(t, c), c
+    return u ? c = u : !o.length && !n && !r ? c = t : (c = {}, o.length && o.forEach(l => Br(c, l, s, !0)), Br(c, t, s)), me(t) && a.set(t, c), c
 }
 
-function Nr(e, t, n, r = !1) {
+function Br(e, t, n, r = !1) {
     const {
         mixins: o,
         extends: a
     } = t;
-    a && Nr(e, a, n, !0), o && o.forEach(s => Nr(e, s, n, !0));
+    a && Br(e, a, n, !0), o && o.forEach(s => Br(e, s, n, !0));
     for (const s in t)
         if (!(r && s === "expose")) {
             const u = ud[s] || n && n[s];
             e[s] = u ? u(e[s], t[s]) : t[s]
         } return e
 }
 const ud = {
-    data: Sa,
-    props: Aa,
-    emits: Aa,
-    methods: Fn,
-    computed: Fn,
+    data: Ta,
+    props: Sa,
+    emits: Sa,
+    methods: xn,
+    computed: xn,
     beforeCreate: Ne,
     created: Ne,
     beforeMount: Ne,
     mounted: Ne,
     beforeUpdate: Ne,
     updated: Ne,
     beforeDestroy: Ne,
     beforeUnmount: Ne,
     destroyed: Ne,
     unmounted: Ne,
     activated: Ne,
     deactivated: Ne,
     errorCaptured: Ne,
     serverPrefetch: Ne,
-    components: Fn,
-    directives: Fn,
+    components: xn,
+    directives: xn,
     watch: dd,
-    provide: Sa,
+    provide: Ta,
     inject: md
 };
 
-function Sa(e, t) {
+function Ta(e, t) {
     return t ? e ? function() {
         return ye(Q(e) ? e.call(this, this) : e, Q(t) ? t.call(this, this) : t)
     } : t : e
 }
 
 function md(e, t) {
-    return Fn(Wo(e), Wo(t))
+    return xn(Uo(e), Uo(t))
 }
 
-function Wo(e) {
+function Uo(e) {
     if (K(e)) {
         const t = {};
         for (let n = 0; n < e.length; n++) t[e[n]] = e[n];
         return t
     }
     return e
 }
 
 function Ne(e, t) {
     return e ? [...new Set([].concat(e, t))] : t
 }
 
-function Fn(e, t) {
+function xn(e, t) {
     return e ? ye(Object.create(null), e, t) : t
 }
 
-function Aa(e, t) {
-    return e ? K(e) && K(t) ? [...new Set([...e, ...t])] : ye(Object.create(null), va(e), va(t ?? {})) : t
+function Sa(e, t) {
+    return e ? K(e) && K(t) ? [...new Set([...e, ...t])] : ye(Object.create(null), ya(e), ya(t ?? {})) : t
 }
 
 function dd(e, t) {
     if (!e) return t;
     if (!t) return e;
     const n = ye(Object.create(null), e);
     for (const r in t) n[r] = Ne(e[r], t[r]);
     return n
 }
 
-function ec() {
+function Jl() {
     return {
         app: null,
         config: {
             isNativeTag: Hu,
             performance: !1,
             globalProperties: {},
             optionMergeStrategies: {},
@@ -1912,15 +1912,15 @@
     }
 }
 let fd = 0;
 
 function _d(e, t) {
     return function(r, o = null) {
         Q(r) || (r = ye({}, r)), o != null && !me(o) && (o = null);
-        const a = ec(),
+        const a = Jl(),
             s = new Set;
         let u = !1;
         const c = a.app = {
             _uid: fd++,
             _component: r,
             _props: o,
             _container: null,
@@ -1942,60 +1942,60 @@
             },
             directive(l, d) {
                 return d ? (a.directives[l] = d, c) : a.directives[l]
             },
             mount(l, d, m) {
                 if (!u) {
                     const f = fe(r, o);
-                    return f.appContext = a, d && t ? t(f, l) : e(f, l, m), u = !0, c._container = l, l.__vue_app__ = c, so(f.component) || f.component.proxy
+                    return f.appContext = a, d && t ? t(f, l) : e(f, l, m), u = !0, c._container = l, l.__vue_app__ = c, ao(f.component) || f.component.proxy
                 }
             },
             unmount() {
                 u && (e(null, c._container), delete c._container.__vue_app__)
             },
             provide(l, d) {
                 return a.provides[l] = d, c
             },
             runWithContext(l) {
-                Hr = c;
+                Nr = c;
                 try {
                     return l()
                 } finally {
-                    Hr = null
+                    Nr = null
                 }
             }
         };
         return c
     }
 }
-let Hr = null;
+let Nr = null;
 
-function Pn(e, t) {
+function An(e, t) {
     if (we) {
         let n = we.provides;
         const r = we.parent && we.parent.provides;
         r === n && (n = we.provides = Object.create(r)), n[e] = t
     }
 }
 
 function ke(e, t, n = !1) {
     const r = we || Oe;
-    if (r || Hr) {
-        const o = r ? r.parent == null ? r.vnode.appContext && r.vnode.appContext.provides : r.parent.provides : Hr._context.provides;
+    if (r || Nr) {
+        const o = r ? r.parent == null ? r.vnode.appContext && r.vnode.appContext.provides : r.parent.provides : Nr._context.provides;
         if (o && e in o) return o[e];
         if (arguments.length > 1) return n && Q(t) ? t.call(r && r.proxy) : t
     }
 }
 
 function pd(e, t, n, r = !1) {
     const o = {},
         a = {};
-    Gr(a, ao, 1), e.propsDefaults = Object.create(null), tc(e, t, o, a);
+    Or(a, io, 1), e.propsDefaults = Object.create(null), ec(e, t, o, a);
     for (const s in e.propsOptions[0]) s in o || (o[s] = void 0);
-    n ? e.props = r ? o : Cl(o) : e.type.props ? e.props = o : e.props = a, e.attrs = a
+    n ? e.props = r ? o : wl(o) : e.type.props ? e.props = o : e.props = a, e.attrs = a
 }
 
 function hd(e, t, n, r) {
     const {
         props: o,
         attrs: a,
         vnode: {
@@ -2004,185 +2004,185 @@
     } = e, u = ee(o), [c] = e.propsOptions;
     let l = !1;
     if ((r || s > 0) && !(s & 16)) {
         if (s & 8) {
             const d = e.vnode.dynamicProps;
             for (let m = 0; m < d.length; m++) {
                 let f = d[m];
-                if (Jr(e.emitsOptions, f)) continue;
+                if (Zr(e.emitsOptions, f)) continue;
                 const _ = t[f];
                 if (c)
                     if (ie(a, f)) _ !== a[f] && (a[f] = _, l = !0);
                     else {
                         const p = gt(f);
-                        o[p] = jo(c, u, p, _, e, !1)
+                        o[p] = Wo(c, u, p, _, e, !1)
                     }
                 else _ !== a[f] && (a[f] = _, l = !0)
             }
         }
     } else {
-        tc(e, t, o, a) && (l = !0);
+        ec(e, t, o, a) && (l = !0);
         let d;
-        for (const m in u)(!t || !ie(t, m) && ((d = nn(m)) === m || !ie(t, d))) && (c ? n && (n[m] !== void 0 || n[d] !== void 0) && (o[m] = jo(c, u, m, void 0, e, !0)) : delete o[m]);
+        for (const m in u)(!t || !ie(t, m) && ((d = nn(m)) === m || !ie(t, d))) && (c ? n && (n[m] !== void 0 || n[d] !== void 0) && (o[m] = Wo(c, u, m, void 0, e, !0)) : delete o[m]);
         if (a !== u)
             for (const m in a)(!t || !ie(t, m)) && (delete a[m], l = !0)
     }
     l && Pt(e, "set", "$attrs")
 }
 
-function tc(e, t, n, r) {
+function ec(e, t, n, r) {
     const [o, a] = e.propsOptions;
     let s = !1,
         u;
     if (t)
         for (let c in t) {
-            if (kr(c)) continue;
+            if (Cr(c)) continue;
             const l = t[c];
             let d;
-            o && ie(o, d = gt(c)) ? !a || !a.includes(d) ? n[d] = l : (u || (u = {}))[d] = l : Jr(e.emitsOptions, c) || (!(c in r) || l !== r[c]) && (r[c] = l, s = !0)
+            o && ie(o, d = gt(c)) ? !a || !a.includes(d) ? n[d] = l : (u || (u = {}))[d] = l : Zr(e.emitsOptions, c) || (!(c in r) || l !== r[c]) && (r[c] = l, s = !0)
         }
     if (a) {
         const c = ee(n),
             l = u || de;
         for (let d = 0; d < a.length; d++) {
             const m = a[d];
-            n[m] = jo(o, c, m, l[m], e, !ie(l, m))
+            n[m] = Wo(o, c, m, l[m], e, !ie(l, m))
         }
     }
     return s
 }
 
-function jo(e, t, n, r, o, a) {
+function Wo(e, t, n, r, o, a) {
     const s = e[n];
     if (s != null) {
         const u = ie(s, "default");
         if (u && r === void 0) {
             const c = s.default;
             if (s.type !== Function && !s.skipFactory && Q(c)) {
                 const {
                     propsDefaults: l
                 } = o;
-                n in l ? r = l[n] : (wn(o), r = l[n] = c.call(null, t), en())
+                n in l ? r = l[n] : (Mn(o), r = l[n] = c.call(null, t), en())
             } else r = c
         }
         s[0] && (a && !u ? r = !1 : s[1] && (r === "" || r === nn(n)) && (r = !0))
     }
     return r
 }
 
-function nc(e, t, n = !1) {
+function tc(e, t, n = !1) {
     const r = t.propsCache,
         o = r.get(e);
     if (o) return o;
     const a = e.props,
         s = {},
         u = [];
     let c = !1;
     if (!Q(e)) {
         const d = m => {
             c = !0;
-            const [f, _] = nc(m, t, !0);
+            const [f, _] = tc(m, t, !0);
             ye(s, f), _ && u.push(..._)
         };
         !n && t.mixins.length && t.mixins.forEach(d), e.extends && d(e.extends), e.mixins && e.mixins.forEach(d)
     }
-    if (!a && !c) return me(e) && r.set(e, vn), vn;
+    if (!a && !c) return me(e) && r.set(e, yn), yn;
     if (K(a))
         for (let d = 0; d < a.length; d++) {
             const m = gt(a[d]);
-            Pa(m) && (s[m] = de)
+            Aa(m) && (s[m] = de)
         } else if (a)
             for (const d in a) {
                 const m = gt(d);
-                if (Pa(m)) {
+                if (Aa(m)) {
                     const f = a[d],
                         _ = s[m] = K(f) || Q(f) ? {
                             type: f
                         } : ye({}, f);
                     if (_) {
-                        const p = wa(Boolean, _.type),
-                            b = wa(String, _.type);
+                        const p = Ma(Boolean, _.type),
+                            b = Ma(String, _.type);
                         _[0] = p > -1, _[1] = b < 0 || p < b, (p > -1 || ie(_, "default")) && u.push(m)
                     }
                 }
             }
     const l = [s, u];
     return me(e) && r.set(e, l), l
 }
 
-function Pa(e) {
+function Aa(e) {
     return e[0] !== "$"
 }
 
-function Ea(e) {
+function Pa(e) {
     const t = e && e.toString().match(/^\s*(function|class) (\w+)/);
     return t ? t[2] : e === null ? "null" : ""
 }
 
-function Ma(e, t) {
-    return Ea(e) === Ea(t)
+function Ea(e, t) {
+    return Pa(e) === Pa(t)
 }
 
-function wa(e, t) {
-    return K(t) ? t.findIndex(n => Ma(n, e)) : Q(t) && Ma(t, e) ? 0 : -1
+function Ma(e, t) {
+    return K(t) ? t.findIndex(n => Ea(n, e)) : Q(t) && Ea(t, e) ? 0 : -1
 }
-const rc = e => e[0] === "_" || e === "$stable",
-    xi = e => K(e) ? e.map(ht) : [ht(e)],
+const nc = e => e[0] === "_" || e === "$stable",
+    Hi = e => K(e) ? e.map(ht) : [ht(e)],
     zd = (e, t, n) => {
         if (t._n) return t;
-        const r = Ul((...o) => xi(t(...o)), n);
+        const r = Vl((...o) => Hi(t(...o)), n);
         return r._c = !1, r
     },
-    oc = (e, t, n) => {
+    rc = (e, t, n) => {
         const r = e._ctx;
         for (const o in e) {
-            if (rc(o)) continue;
+            if (nc(o)) continue;
             const a = e[o];
             if (Q(a)) t[o] = zd(o, a, r);
             else if (a != null) {
-                const s = xi(a);
+                const s = Hi(a);
                 t[o] = () => s
             }
         }
     },
-    ic = (e, t) => {
-        const n = xi(t);
+    oc = (e, t) => {
+        const n = Hi(t);
         e.slots.default = () => n
     },
     bd = (e, t) => {
         if (e.vnode.shapeFlag & 32) {
             const n = t._;
-            n ? (e.slots = ee(t), Gr(t, "_", n)) : oc(t, e.slots = {})
-        } else e.slots = {}, t && ic(e, t);
-        Gr(e.slots, ao, 1)
+            n ? (e.slots = ee(t), Or(t, "_", n)) : rc(t, e.slots = {})
+        } else e.slots = {}, t && oc(e, t);
+        Or(e.slots, io, 1)
     },
     gd = (e, t, n) => {
         const {
             vnode: r,
             slots: o
         } = e;
         let a = !0,
             s = de;
         if (r.shapeFlag & 32) {
             const u = t._;
-            u ? n && u === 1 ? a = !1 : (ye(o, t), !n && u === 1 && delete o._) : (a = !t.$stable, oc(t, o)), s = t
-        } else t && (ic(e, t), s = {
+            u ? n && u === 1 ? a = !1 : (ye(o, t), !n && u === 1 && delete o._) : (a = !t.$stable, rc(t, o)), s = t
+        } else t && (oc(e, t), s = {
             default: 1
         });
         if (a)
-            for (const u in o) !rc(u) && !(u in s) && delete o[u]
+            for (const u in o) !nc(u) && !(u in s) && delete o[u]
     };
 
-function qo(e, t, n, r, o = !1) {
+function jo(e, t, n, r, o = !1) {
     if (K(e)) {
-        e.forEach((f, _) => qo(f, t && (K(t) ? t[_] : t), n, r, o));
+        e.forEach((f, _) => jo(f, t && (K(t) ? t[_] : t), n, r, o));
         return
     }
-    if (Vn(r) && !o) return;
-    const a = r.shapeFlag & 4 ? so(r.component) || r.component.proxy : r.el,
+    if (Fn(r) && !o) return;
+    const a = r.shapeFlag & 4 ? ao(r.component) || r.component.proxy : r.el,
         s = o ? null : a,
         {
             i: u,
             r: c
         } = e,
         l = t && t.r,
         d = u.refs === de ? u.refs = {} : u.refs,
@@ -2191,29 +2191,29 @@
     else {
         const f = be(c),
             _ = Ae(c);
         if (f || _) {
             const p = () => {
                 if (e.f) {
                     const b = f ? ie(m, c) ? m[c] : d[c] : c.value;
-                    o ? K(b) && bi(b, a) : K(b) ? b.includes(a) || b.push(a) : f ? (d[c] = [a], ie(m, c) && (m[c] = d[c])) : (c.value = [a], e.k && (d[e.k] = c.value))
+                    o ? K(b) && zi(b, a) : K(b) ? b.includes(a) || b.push(a) : f ? (d[c] = [a], ie(m, c) && (m[c] = d[c])) : (c.value = [a], e.k && (d[e.k] = c.value))
                 } else f ? (d[c] = s, ie(m, c) && (m[c] = s)) : _ && (c.value = s, e.k && (d[e.k] = s))
             };
             s ? (p.id = -1, Ue(p, n)) : p()
         }
     }
 }
 const Ue = qm;
 
 function yd(e) {
     return vd(e)
 }
 
 function vd(e, t) {
-    const n = Bo();
+    const n = Lo();
     n.__VUE__ = !0;
     const {
         insert: r,
         remove: o,
         patchProp: a,
         createElement: s,
         createText: u,
@@ -2229,30 +2229,30 @@
         h && !Xt(h, z) && (E = w(h), Ge(h, k, D, !0), h = null), z.patchFlag === -2 && (G = !1, z.dynamicChildren = null);
         const {
             type: C,
             ref: y,
             shapeFlag: S
         } = z;
         switch (C) {
-            case mr:
+            case ur:
                 T(h, z, g, E);
                 break;
             case nt:
                 v(h, z, g, E);
                 break;
-            case Ao:
+            case So:
                 h == null && A(z, g, E, B);
                 break;
             case He:
                 x(h, z, g, E, k, D, B, O, G);
                 break;
             default:
                 S & 1 ? M(h, z, g, E, k, D, B, O, G) : S & 6 ? te(h, z, g, E, k, D, B, O, G) : (S & 64 || S & 128) && C.process(h, z, g, E, k, D, B, O, G, R)
         }
-        y != null && k && qo(y, h && h.ref, D, z || h, !z)
+        y != null && k && jo(y, h && h.ref, D, z || h, !z)
     }, T = (h, z, g, E) => {
         if (h == null) r(z.el = u(z.children), g, E);
         else {
             const k = z.el = h.el;
             z.children !== h.children && l(k, z.children)
         }
     }, v = (h, z, g, E) => {
@@ -2281,15 +2281,15 @@
             type: y,
             props: S,
             shapeFlag: F,
             transition: W,
             dirs: Z
         } = h;
         if (G = h.el = s(h.type, D, S && S.is, S), F & 8 ? d(G, h.children) : F & 16 && L(h.children, G, null, E, k, D && y !== "foreignObject", B, O), Z && Vt(h, null, E, "created"), j(G, h, h.scopeId, B, E), S) {
-            for (const J in S) J !== "value" && !kr(J) && a(G, J, null, S[J], D, h.children, E, k, Pe);
+            for (const J in S) J !== "value" && !Cr(J) && a(G, J, null, S[J], D, h.children, E, k, Pe);
             "value" in S && a(G, "value", null, S.value), (C = S.onVnodeBeforeMount) && pt(C, E, h)
         }
         Z && Vt(h, null, E, "beforeMount");
         const le = (!k || k && !k.pendingBranch) && W && !W.persisted;
         le && W.beforeEnter(G), r(G, z, g), ((C = S && S.onVnodeMounted) || le || Z) && Ue(() => {
             C && pt(C, E, h), le && W.enter(G), Z && Vt(h, null, E, "mounted")
         }, k)
@@ -2343,37 +2343,37 @@
                 C = z[O],
                 y = G.el && (G.type === He || !Xt(G, C) || G.shapeFlag & 70) ? m(G.el) : g;
             b(G, C, y, null, E, k, D, B, !0)
         }
     }, Y = (h, z, g, E, k, D, B) => {
         if (g !== E) {
             if (g !== de)
-                for (const O in g) !kr(O) && !(O in E) && a(h, O, g[O], null, B, z.children, k, D, Pe);
+                for (const O in g) !Cr(O) && !(O in E) && a(h, O, g[O], null, B, z.children, k, D, Pe);
             for (const O in E) {
-                if (kr(O)) continue;
+                if (Cr(O)) continue;
                 const G = E[O],
                     C = g[O];
                 G !== C && O !== "value" && a(h, O, C, G, B, z.children, k, D, Pe)
             }
             "value" in E && a(h, "value", g.value, E.value)
         }
     }, x = (h, z, g, E, k, D, B, O, G) => {
         const C = z.el = h ? h.el : u(""),
             y = z.anchor = h ? h.anchor : u("");
         let {
             patchFlag: S,
             dynamicChildren: F,
             slotScopeIds: W
         } = z;
-        W && (O = O ? O.concat(W) : W), h == null ? (r(C, g, E), r(y, g, E), L(z.children, g, y, k, D, B, O, G)) : S > 0 && S & 64 && F && h.dynamicChildren ? ($(h.dynamicChildren, F, g, k, D, B, O), (z.key != null || k && z === k.subTree) && Fi(h, z, !0)) : oe(h, z, g, y, k, D, B, O, G)
+        W && (O = O ? O.concat(W) : W), h == null ? (r(C, g, E), r(y, g, E), L(z.children, g, y, k, D, B, O, G)) : S > 0 && S & 64 && F && h.dynamicChildren ? ($(h.dynamicChildren, F, g, k, D, B, O), (z.key != null || k && z === k.subTree) && xi(h, z, !0)) : oe(h, z, g, y, k, D, B, O, G)
     }, te = (h, z, g, E, k, D, B, O, G) => {
         z.slotScopeIds = O, h == null ? z.shapeFlag & 512 ? k.ctx.activate(z, g, E, B, G) : De(z, g, E, k, D, B, G) : ot(h, z, G)
     }, De = (h, z, g, E, k, D, B) => {
         const O = h.component = Id(h, E, k);
-        if (ro(h) && (O.ctx.renderer = R), Od(O), O.asyncDep) {
+        if (no(h) && (O.ctx.renderer = R), Od(O), O.asyncDep) {
             if (k && k.registerDep(O, _e), !h.el) {
                 const G = O.subTree = fe(nt);
                 v(null, G, z, g)
             }
             return
         }
         _e(O, h, z, g, k, D, B)
@@ -2391,50 +2391,50 @@
                     let {
                         next: y,
                         bu: S,
                         u: F,
                         parent: W,
                         vnode: Z
                     } = h, le = y, J;
-                    Ut(h, !1), y ? (y.el = Z.el, ne(h, y, B)) : y = Z, S && yo(S), (J = y.props && y.props.onVnodeBeforeUpdate) && pt(J, W, y, Z), Ut(h, !0);
-                    const he = vo(h),
+                    Ut(h, !1), y ? (y.el = Z.el, ne(h, y, B)) : y = Z, S && go(S), (J = y.props && y.props.onVnodeBeforeUpdate) && pt(J, W, y, Z), Ut(h, !0);
+                    const he = yo(h),
                         Ze = h.subTree;
                     h.subTree = he, b(Ze, he, m(Ze.el), w(Ze), h, k, D), y.el = he.el, le === null && Wm(h, he.el), F && Ue(F, k), (J = y.props && y.props.onVnodeUpdated) && Ue(() => pt(J, W, y, Z), k)
                 } else {
                     let y;
                     const {
                         el: S,
                         props: F
                     } = z, {
                         bm: W,
                         m: Z,
                         parent: le
-                    } = h, J = Vn(z);
-                    if (Ut(h, !1), W && yo(W), !J && (y = F && F.onVnodeBeforeMount) && pt(y, le, z), Ut(h, !0), S && se) {
+                    } = h, J = Fn(z);
+                    if (Ut(h, !1), W && go(W), !J && (y = F && F.onVnodeBeforeMount) && pt(y, le, z), Ut(h, !0), S && se) {
                         const he = () => {
-                            h.subTree = vo(h), se(S, h.subTree, h, k, null)
+                            h.subTree = yo(h), se(S, h.subTree, h, k, null)
                         };
                         J ? z.type.__asyncLoader().then(() => !h.isUnmounted && he()) : he()
                     } else {
-                        const he = h.subTree = vo(h);
+                        const he = h.subTree = yo(h);
                         b(null, he, g, E, h, k, D), z.el = he.el
                     }
                     if (Z && Ue(Z, k), !J && (y = F && F.onVnodeMounted)) {
                         const he = z;
                         Ue(() => pt(y, le, he), k)
-                    }(z.shapeFlag & 256 || le && Vn(le.vnode) && le.vnode.shapeFlag & 256) && h.a && Ue(h.a, k), h.isMounted = !0, z = g = E = null
+                    }(z.shapeFlag & 256 || le && Fn(le.vnode) && le.vnode.shapeFlag & 256) && h.a && Ue(h.a, k), h.isMounted = !0, z = g = E = null
                 }
             },
-            G = h.effect = new Ai(O, () => Oi(C), h.scope),
+            G = h.effect = new Si(O, () => Ii(C), h.scope),
             C = h.update = () => G.run();
         C.id = h.uid, Ut(h, !0), C()
     }, ne = (h, z, g) => {
         z.component = h;
         const E = h.vnode.props;
-        h.vnode = z, h.next = null, hd(h, z.props, E, g), gd(h, z.children, g), Dn(), za(), In()
+        h.vnode = z, h.next = null, hd(h, z.props, E, g), gd(h, z.children, g), kn(), ha(), Dn()
     }, oe = (h, z, g, E, k, D, B, O, G = !1) => {
         const C = h && h.children,
             y = h ? h.shapeFlag : 0,
             S = z.children,
             {
                 patchFlag: F,
                 shapeFlag: W
@@ -2446,15 +2446,15 @@
             } else if (F & 256) {
                 it(C, S, g, E, k, D, B, O, G);
                 return
             }
         }
         W & 8 ? (y & 16 && Pe(C, k, D), S !== C && d(g, S)) : y & 16 ? W & 16 ? ft(C, S, g, E, k, D, B, O, G) : Pe(C, k, D, !0) : (y & 8 && d(g, ""), W & 16 && L(S, g, E, k, D, B, O, G))
     }, it = (h, z, g, E, k, D, B, O, G) => {
-        h = h || vn, z = z || vn;
+        h = h || yn, z = z || yn;
         const C = h.length,
             y = z.length,
             S = Math.min(C, y);
         let F;
         for (F = 0; F < S; F++) {
             const W = z[F] = G ? It(z[F]) : ht(z[F]);
             b(h[F], W, g, null, k, D, B, O, G)
@@ -2494,38 +2494,38 @@
             for (C = Z; C <= F; C++) {
                 const je = z[C] = G ? It(z[C]) : ht(z[C]);
                 je.key != null && le.set(je.key, C)
             }
             let J, he = 0;
             const Ze = F - Z + 1;
             let sn = !1,
-                aa = 0;
-            const Gn = new Array(Ze);
-            for (C = 0; C < Ze; C++) Gn[C] = 0;
+                ia = 0;
+            const On = new Array(Ze);
+            for (C = 0; C < Ze; C++) On[C] = 0;
             for (C = W; C <= S; C++) {
                 const je = h[C];
                 if (he >= Ze) {
                     Ge(je, k, D, !0);
                     continue
                 }
                 let _t;
                 if (je.key != null) _t = le.get(je.key);
                 else
                     for (J = Z; J <= F; J++)
-                        if (Gn[J - Z] === 0 && Xt(je, z[J])) {
+                        if (On[J - Z] === 0 && Xt(je, z[J])) {
                             _t = J;
                             break
-                        } _t === void 0 ? Ge(je, k, D, !0) : (Gn[_t - Z] = C + 1, _t >= aa ? aa = _t : sn = !0, b(je, z[_t], g, null, k, D, B, O, G), he++)
+                        } _t === void 0 ? Ge(je, k, D, !0) : (On[_t - Z] = C + 1, _t >= ia ? ia = _t : sn = !0, b(je, z[_t], g, null, k, D, B, O, G), he++)
             }
-            const sa = sn ? Td(Gn) : vn;
-            for (J = sa.length - 1, C = Ze - 1; C >= 0; C--) {
+            const aa = sn ? Td(On) : yn;
+            for (J = aa.length - 1, C = Ze - 1; C >= 0; C--) {
                 const je = Z + C,
                     _t = z[je],
-                    la = je + 1 < y ? z[je + 1].el : E;
-                Gn[C] === 0 ? b(null, _t, g, la, k, D, B, O, G) : sn && (J < 0 || C !== sa[J] ? Qe(_t, g, la, 2) : J--)
+                    sa = je + 1 < y ? z[je + 1].el : E;
+                On[C] === 0 ? b(null, _t, g, sa, k, D, B, O, G) : sn && (J < 0 || C !== aa[J] ? Qe(_t, g, sa, 2) : J--)
             }
         }
     }, Qe = (h, z, g, E, k = null) => {
         const {
             el: D,
             type: B,
             transition: O,
@@ -2546,15 +2546,15 @@
         }
         if (B === He) {
             r(D, z, g);
             for (let S = 0; S < G.length; S++) Qe(G[S], z, g, E);
             r(h.anchor, z, g);
             return
         }
-        if (B === Ao) {
+        if (B === So) {
             I(h, z, g);
             return
         }
         if (E !== 2 && C & 1 && O)
             if (E === 0) O.beforeEnter(D), r(D, z, g), Ue(() => O.enter(D), k);
             else {
                 const {
@@ -2576,20 +2576,20 @@
             ref: O,
             children: G,
             dynamicChildren: C,
             shapeFlag: y,
             patchFlag: S,
             dirs: F
         } = h;
-        if (O != null && qo(O, null, g, h, !0), y & 256) {
+        if (O != null && jo(O, null, g, h, !0), y & 256) {
             z.ctx.deactivate(h);
             return
         }
         const W = y & 1 && F,
-            Z = !Vn(h);
+            Z = !Fn(h);
         let le;
         if (Z && (le = B && B.onVnodeBeforeUnmount) && pt(le, z, h), y & 6) an(h.component, g, E);
         else {
             if (y & 128) {
                 h.suspense.unmount(g, E);
                 return
             }
@@ -2604,15 +2604,15 @@
             anchor: E,
             transition: k
         } = h;
         if (z === He) {
             Mt(g, E);
             return
         }
-        if (z === Ao) {
+        if (z === So) {
             P(h);
             return
         }
         const D = () => {
             o(g), k && !k.persisted && k.afterLeave && k.afterLeave()
         };
         if (h.shapeFlag & 1 && k && !k.persisted) {
@@ -2630,21 +2630,21 @@
         const {
             bum: E,
             scope: k,
             update: D,
             subTree: B,
             um: O
         } = h;
-        E && yo(E), k.stop(), D && (D.active = !1, Ge(B, h, z, g)), O && Ue(O, z), Ue(() => {
+        E && go(E), k.stop(), D && (D.active = !1, Ge(B, h, z, g)), O && Ue(O, z), Ue(() => {
             h.isUnmounted = !0
         }, z), z && z.pendingBranch && !z.isUnmounted && h.asyncDep && !h.asyncResolved && h.suspenseId === z.pendingId && (z.deps--, z.deps === 0 && z.resolve())
     }, Pe = (h, z, g, E = !1, k = !1, D = 0) => {
         for (let B = D; B < h.length; B++) Ge(h[B], z, g, E, k)
     }, w = h => h.shapeFlag & 6 ? w(h.component.subTree) : h.shapeFlag & 128 ? h.suspense.next() : f(h.anchor || h.el), H = (h, z, g) => {
-        h == null ? z._vnode && Ge(z._vnode, null, null, !0) : b(z._vnode || null, h, z, null, null, null, g), za(), xl(), z._vnode = h
+        h == null ? z._vnode && Ge(z._vnode, null, null, !0) : b(z._vnode || null, h, z, null, null, null, g), ha(), Hl(), z._vnode = h
     }, R = {
         p: b,
         um: Ge,
         m: Qe,
         r: Ft,
         mt: De,
         mc: L,
@@ -2664,22 +2664,22 @@
 function Ut({
     effect: e,
     update: t
 }, n) {
     e.allowRecurse = t.allowRecurse = n
 }
 
-function Fi(e, t, n = !1) {
+function xi(e, t, n = !1) {
     const r = e.children,
         o = t.children;
     if (K(r) && K(o))
         for (let a = 0; a < r.length; a++) {
             const s = r[a];
             let u = o[a];
-            u.shapeFlag & 1 && !u.dynamicChildren && ((u.patchFlag <= 0 || u.patchFlag === 32) && (u = o[a] = It(o[a]), u.el = s.el), n || Fi(s, u)), u.type === mr && (u.el = s.el)
+            u.shapeFlag & 1 && !u.dynamicChildren && ((u.patchFlag <= 0 || u.patchFlag === 32) && (u = o[a] = It(o[a]), u.el = s.el), n || xi(s, u)), u.type === ur && (u.el = s.el)
         }
 }
 
 function Td(e) {
     const t = e.slice(),
         n = [0];
     let r, o, a, s, u;
@@ -2695,17 +2695,17 @@
             l < e[n[a]] && (a > 0 && (t[r] = n[a - 1]), n[a] = r)
         }
     }
     for (a = n.length, s = n[a - 1]; a-- > 0;) n[a] = s, s = t[s];
     return n
 }
 const Sd = e => e.__isTeleport,
-    Wn = e => e && (e.disabled || e.disabled === ""),
-    Ca = e => typeof SVGElement < "u" && e instanceof SVGElement,
-    Ko = (e, t) => {
+    Un = e => e && (e.disabled || e.disabled === ""),
+    wa = e => typeof SVGElement < "u" && e instanceof SVGElement,
+    qo = (e, t) => {
         const n = e && e.to;
         return be(n) ? t ? t(n) : null : n
     },
     Ad = {
         __isTeleport: !0,
         process(e, t, n, r, o, a, s, u, c, l) {
             const {
@@ -2714,46 +2714,46 @@
                 pbc: f,
                 o: {
                     insert: _,
                     querySelector: p,
                     createText: b,
                     createComment: T
                 }
-            } = l, v = Wn(t.props);
+            } = l, v = Un(t.props);
             let {
                 shapeFlag: A,
                 children: I,
                 dynamicChildren: P
             } = t;
             if (e == null) {
                 const M = t.el = b(""),
                     N = t.anchor = b("");
                 _(M, n, r), _(N, n, r);
-                const j = t.target = Ko(t.props, p),
+                const j = t.target = qo(t.props, p),
                     L = t.targetAnchor = b("");
-                j && (_(L, j), s = s || Ca(j));
+                j && (_(L, j), s = s || wa(j));
                 const X = ($, Y) => {
                     A & 16 && d(I, $, Y, o, a, s, u, c)
                 };
                 v ? X(n, N) : j && X(j, L)
             } else {
                 t.el = e.el;
                 const M = t.anchor = e.anchor,
                     N = t.target = e.target,
                     j = t.targetAnchor = e.targetAnchor,
-                    L = Wn(e.props),
+                    L = Un(e.props),
                     X = L ? n : N,
                     $ = L ? M : j;
-                if (s = s || Ca(N), P ? (f(e.dynamicChildren, P, X, o, a, s, u), Fi(e, t, !0)) : c || m(e, t, X, $, o, a, s, u, !1), v) L || yr(t, n, M, l, 1);
+                if (s = s || wa(N), P ? (f(e.dynamicChildren, P, X, o, a, s, u), xi(e, t, !0)) : c || m(e, t, X, $, o, a, s, u, !1), v) L || gr(t, n, M, l, 1);
                 else if ((t.props && t.props.to) !== (e.props && e.props.to)) {
-                    const Y = t.target = Ko(t.props, p);
-                    Y && yr(t, Y, null, l, 0)
-                } else L && yr(t, N, j, l, 1)
+                    const Y = t.target = qo(t.props, p);
+                    Y && gr(t, Y, null, l, 0)
+                } else L && gr(t, N, j, l, 1)
             }
-            ac(t)
+            ic(t)
         },
         remove(e, t, n, r, {
             um: o,
             o: {
                 remove: a
             }
         }, s) {
@@ -2761,140 +2761,140 @@
                 shapeFlag: u,
                 children: c,
                 anchor: l,
                 targetAnchor: d,
                 target: m,
                 props: f
             } = e;
-            if (m && a(d), (s || !Wn(f)) && (a(l), u & 16))
+            if (m && a(d), (s || !Un(f)) && (a(l), u & 16))
                 for (let _ = 0; _ < c.length; _++) {
                     const p = c[_];
                     o(p, t, n, !0, !!p.dynamicChildren)
                 }
         },
-        move: yr,
+        move: gr,
         hydrate: Pd
     };
 
-function yr(e, t, n, {
+function gr(e, t, n, {
     o: {
         insert: r
     },
     m: o
 }, a = 2) {
     a === 0 && r(e.targetAnchor, t, n);
     const {
         el: s,
         anchor: u,
         shapeFlag: c,
         children: l,
         props: d
     } = e, m = a === 2;
-    if (m && r(s, t, n), (!m || Wn(d)) && c & 16)
+    if (m && r(s, t, n), (!m || Un(d)) && c & 16)
         for (let f = 0; f < l.length; f++) o(l[f], t, n, 2);
     m && r(u, t, n)
 }
 
 function Pd(e, t, n, r, o, a, {
     o: {
         nextSibling: s,
         parentNode: u,
         querySelector: c
     }
 }, l) {
-    const d = t.target = Ko(t.props, c);
+    const d = t.target = qo(t.props, c);
     if (d) {
         const m = d._lpa || d.firstChild;
         if (t.shapeFlag & 16)
-            if (Wn(t.props)) t.anchor = l(s(e), t, u(e), n, r, o, a), t.targetAnchor = m;
+            if (Un(t.props)) t.anchor = l(s(e), t, u(e), n, r, o, a), t.targetAnchor = m;
             else {
                 t.anchor = s(e);
                 let f = m;
                 for (; f;)
                     if (f = s(f), f && f.nodeType === 8 && f.data === "teleport anchor") {
                         t.targetAnchor = f, d._lpa = t.targetAnchor && s(t.targetAnchor);
                         break
                     } l(m, t, d, n, r, o, a)
-            } ac(t)
+            } ic(t)
     }
     return t.anchor && s(t.anchor)
 }
 const ob = Ad;
 
-function ac(e) {
+function ic(e) {
     const t = e.ctx;
     if (t && t.ut) {
         let n = e.children[0].el;
         for (; n !== e.targetAnchor;) n.nodeType === 1 && n.setAttribute("data-v-owner", t.uid), n = n.nextSibling;
         t.ut()
     }
 }
 const He = Symbol.for("v-fgt"),
-    mr = Symbol.for("v-txt"),
+    ur = Symbol.for("v-txt"),
     nt = Symbol.for("v-cmt"),
-    Ao = Symbol.for("v-stc"),
-    jn = [];
+    So = Symbol.for("v-stc"),
+    Wn = [];
 let ct = null;
 
-function Vi(e = !1) {
-    jn.push(ct = e ? null : [])
+function Fi(e = !1) {
+    Wn.push(ct = e ? null : [])
 }
 
 function Ed() {
-    jn.pop(), ct = jn[jn.length - 1] || null
+    Wn.pop(), ct = Wn[Wn.length - 1] || null
 }
-let nr = 1;
+let tr = 1;
 
-function ka(e) {
-    nr += e
+function Ca(e) {
+    tr += e
 }
 
-function sc(e) {
-    return e.dynamicChildren = nr > 0 ? ct || vn : null, Ed(), nr > 0 && ct && ct.push(e), e
+function ac(e) {
+    return e.dynamicChildren = tr > 0 ? ct || yn : null, Ed(), tr > 0 && ct && ct.push(e), e
 }
 
 function ib(e, t, n, r, o, a) {
-    return sc(cc(e, t, n, r, o, a, !0))
+    return ac(lc(e, t, n, r, o, a, !0))
 }
 
-function Ui(e, t, n, r, o) {
-    return sc(fe(e, t, n, r, o, !0))
+function Vi(e, t, n, r, o) {
+    return ac(fe(e, t, n, r, o, !0))
 }
 
-function xr(e) {
+function Hr(e) {
     return e ? e.__v_isVNode === !0 : !1
 }
 
 function Xt(e, t) {
     return e.type === t.type && e.key === t.key
 }
-const ao = "__vInternal",
-    lc = ({
+const io = "__vInternal",
+    sc = ({
         key: e
     }) => e ?? null,
-    Ir = ({
+    Dr = ({
         ref: e,
         ref_key: t,
         ref_for: n
     }) => (typeof e == "number" && (e = "" + e), e != null ? be(e) || Ae(e) || Q(e) ? {
         i: Oe,
         r: e,
         k: t,
         f: !!n
     } : e : null);
 
-function cc(e, t = null, n = null, r = 0, o = null, a = e === He ? 0 : 1, s = !1, u = !1) {
+function lc(e, t = null, n = null, r = 0, o = null, a = e === He ? 0 : 1, s = !1, u = !1) {
     const c = {
         __v_isVNode: !0,
         __v_skip: !0,
         type: e,
         props: t,
-        key: t && lc(t),
-        ref: t && Ir(t),
-        scopeId: eo,
+        key: t && sc(t),
+        ref: t && Dr(t),
+        scopeId: Jr,
         slotScopeIds: null,
         children: n,
         component: null,
         suspense: null,
         ssContent: null,
         ssFallback: null,
         dirs: null,
@@ -2907,53 +2907,53 @@
         shapeFlag: a,
         patchFlag: r,
         dynamicProps: o,
         dynamicChildren: null,
         appContext: null,
         ctx: Oe
     };
-    return u ? (Wi(c, n), a & 128 && e.normalize(c)) : n && (c.shapeFlag |= be(n) ? 8 : 16), nr > 0 && !s && ct && (c.patchFlag > 0 || a & 6) && c.patchFlag !== 32 && ct.push(c), c
+    return u ? (Ui(c, n), a & 128 && e.normalize(c)) : n && (c.shapeFlag |= be(n) ? 8 : 16), tr > 0 && !s && ct && (c.patchFlag > 0 || a & 6) && c.patchFlag !== 32 && ct.push(c), c
 }
 const fe = Md;
 
 function Md(e, t = null, n = null, r = 0, o = null, a = !1) {
-    if ((!e || e === Ql) && (e = nt), xr(e)) {
+    if ((!e || e === Yl) && (e = nt), Hr(e)) {
         const u = Nt(e, t, !0);
-        return n && Wi(u, n), nr > 0 && !a && ct && (u.shapeFlag & 6 ? ct[ct.indexOf(e)] = u : ct.push(u)), u.patchFlag |= -2, u
+        return n && Ui(u, n), tr > 0 && !a && ct && (u.shapeFlag & 6 ? ct[ct.indexOf(e)] = u : ct.push(u)), u.patchFlag |= -2, u
     }
     if (Nd(e) && (e = e.__vccOpts), t) {
         t = wd(t);
         let {
             class: u,
             style: c
         } = t;
-        u && !be(u) && (t.class = Ti(u)), me(c) && (Dl(c) && !K(c) && (c = ye({}, c)), t.style = vi(c))
+        u && !be(u) && (t.class = vi(u)), me(c) && (kl(c) && !K(c) && (c = ye({}, c)), t.style = yi(c))
     }
     const s = be(e) ? 1 : jm(e) ? 128 : Sd(e) ? 64 : me(e) ? 4 : Q(e) ? 2 : 0;
-    return cc(e, t, n, r, o, s, a, !0)
+    return lc(e, t, n, r, o, s, a, !0)
 }
 
 function wd(e) {
-    return e ? Dl(e) || ao in e ? ye({}, e) : e : null
+    return e ? kl(e) || io in e ? ye({}, e) : e : null
 }
 
 function Nt(e, t, n = !1) {
     const {
         props: r,
         ref: o,
         patchFlag: a,
         children: s
-    } = e, u = t ? uc(r || {}, t) : r;
+    } = e, u = t ? cc(r || {}, t) : r;
     return {
         __v_isVNode: !0,
         __v_skip: !0,
         type: e.type,
         props: u,
-        key: u && lc(u),
-        ref: t && t.ref ? n && o ? K(o) ? o.concat(Ir(t)) : [o, Ir(t)] : Ir(t) : o,
+        key: u && sc(u),
+        ref: t && t.ref ? n && o ? K(o) ? o.concat(Dr(t)) : [o, Dr(t)] : Dr(t) : o,
         scopeId: e.scopeId,
         slotScopeIds: e.slotScopeIds,
         children: s,
         target: e.target,
         targetAnchor: e.targetAnchor,
         staticCount: e.staticCount,
         shapeFlag: e.shapeFlag,
@@ -2971,73 +2971,73 @@
         anchor: e.anchor,
         ctx: e.ctx,
         ce: e.ce
     }
 }
 
 function Cd(e = " ", t = 0) {
-    return fe(mr, null, e, t)
+    return fe(ur, null, e, t)
 }
 
 function ab(e = "", t = !1) {
-    return t ? (Vi(), Ui(nt, null, e)) : fe(nt, null, e)
+    return t ? (Fi(), Vi(nt, null, e)) : fe(nt, null, e)
 }
 
 function ht(e) {
-    return e == null || typeof e == "boolean" ? fe(nt) : K(e) ? fe(He, null, e.slice()) : typeof e == "object" ? It(e) : fe(mr, null, String(e))
+    return e == null || typeof e == "boolean" ? fe(nt) : K(e) ? fe(He, null, e.slice()) : typeof e == "object" ? It(e) : fe(ur, null, String(e))
 }
 
 function It(e) {
     return e.el === null && e.patchFlag !== -1 || e.memo ? e : Nt(e)
 }
 
-function Wi(e, t) {
+function Ui(e, t) {
     let n = 0;
     const {
         shapeFlag: r
     } = e;
     if (t == null) t = null;
     else if (K(t)) n = 16;
     else if (typeof t == "object")
         if (r & 65) {
             const o = t.default;
-            o && (o._c && (o._d = !1), Wi(e, o()), o._c && (o._d = !0));
+            o && (o._c && (o._d = !1), Ui(e, o()), o._c && (o._d = !0));
             return
         } else {
             n = 32;
             const o = t._;
-            !o && !(ao in t) ? t._ctx = Oe : o === 3 && Oe && (Oe.slots._ === 1 ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024))
+            !o && !(io in t) ? t._ctx = Oe : o === 3 && Oe && (Oe.slots._ === 1 ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024))
         }
     else Q(t) ? (t = {
         default: t,
         _ctx: Oe
     }, n = 32) : (t = String(t), r & 64 ? (n = 16, t = [Cd(t)]) : n = 8);
     e.children = t, e.shapeFlag |= n
 }
 
-function uc(...e) {
+function cc(...e) {
     const t = {};
     for (let n = 0; n < e.length; n++) {
         const r = e[n];
         for (const o in r)
-            if (o === "class") t.class !== r.class && (t.class = Ti([t.class, r.class]));
-            else if (o === "style") t.style = vi([t.style, r.style]);
-        else if (Xr(o)) {
+            if (o === "class") t.class !== r.class && (t.class = vi([t.class, r.class]));
+            else if (o === "style") t.style = yi([t.style, r.style]);
+        else if (Kr(o)) {
             const a = t[o],
                 s = r[o];
             s && a !== s && !(K(a) && a.includes(s)) && (t[o] = a ? [].concat(a, s) : s)
         } else o !== "" && (t[o] = r[o])
     }
     return t
 }
 
 function pt(e, t, n, r = null) {
     tt(e, t, 7, [n, r])
 }
-const kd = ec();
+const kd = Jl();
 let Dd = 0;
 
 function Id(e, t, n) {
     const r = e.type,
         o = (t ? t.appContext : e.appContext) || kd,
         a = {
             uid: Dd++,
@@ -3046,27 +3046,27 @@
             parent: t,
             appContext: o,
             root: null,
             next: null,
             subTree: null,
             effect: null,
             update: null,
-            scope: new zl(!0),
+            scope: new hl(!0),
             render: null,
             proxy: null,
             exposed: null,
             exposeProxy: null,
             withProxy: null,
             provides: t ? t.provides : Object.create(o.provides),
             accessCache: null,
             renderCache: [],
             components: null,
             directives: null,
-            propsOptions: nc(r, o),
-            emitsOptions: Vl(r, o),
+            propsOptions: tc(r, o),
+            emitsOptions: Fl(r, o),
             emit: null,
             emitted: null,
             propsDefaults: de,
             inheritAttrs: r.inheritAttrs,
             ctx: de,
             data: de,
             props: de,
@@ -3100,90 +3100,90 @@
             sp: null
         };
     return a.ctx = {
         _: a
     }, a.root = t ? t.root : a, a.emit = xm.bind(null, a), e.ce && e.ce(a), a
 }
 let we = null;
-const On = () => we || Oe;
-let ji, ln, Da = "__VUE_INSTANCE_SETTERS__";
-(ln = Bo()[Da]) || (ln = Bo()[Da] = []), ln.push(e => we = e), ji = e => {
+const In = () => we || Oe;
+let Wi, ln, ka = "__VUE_INSTANCE_SETTERS__";
+(ln = Lo()[ka]) || (ln = Lo()[ka] = []), ln.push(e => we = e), Wi = e => {
     ln.length > 1 ? ln.forEach(t => t(e)) : ln[0](e)
 };
-const wn = e => {
-        ji(e), e.scope.on()
+const Mn = e => {
+        Wi(e), e.scope.on()
     },
     en = () => {
-        we && we.scope.off(), ji(null)
+        we && we.scope.off(), Wi(null)
     };
 
-function mc(e) {
+function uc(e) {
     return e.vnode.shapeFlag & 4
 }
-let rr = !1;
+let nr = !1;
 
 function Od(e, t = !1) {
-    rr = t;
+    nr = t;
     const {
         props: n,
         children: r
-    } = e.vnode, o = mc(e);
+    } = e.vnode, o = uc(e);
     pd(e, n, o, t), bd(e, r);
     const a = o ? Gd(e, t) : void 0;
-    return rr = !1, a
+    return nr = !1, a
 }
 
 function Gd(e, t) {
     const n = e.type;
-    e.accessCache = Object.create(null), e.proxy = Il(new Proxy(e.ctx, sd));
+    e.accessCache = Object.create(null), e.proxy = Dl(new Proxy(e.ctx, sd));
     const {
         setup: r
     } = n;
     if (r) {
         const o = e.setupContext = r.length > 1 ? Ld(e) : null;
-        wn(e), Dn();
+        Mn(e), kn();
         const a = Rt(r, e, 0, [e.props, o]);
-        if (In(), en(), dl(a)) {
+        if (Dn(), en(), ml(a)) {
             if (a.then(en, en), t) return a.then(s => {
-                Ia(e, s, t)
+                Da(e, s, t)
             }).catch(s => {
-                Zr(s, e, 0)
+                Qr(s, e, 0)
             });
             e.asyncDep = a
-        } else Ia(e, a, t)
-    } else dc(e, t)
+        } else Da(e, a, t)
+    } else mc(e, t)
 }
 
-function Ia(e, t, n) {
-    Q(t) ? e.type.__ssrInlineRender ? e.ssrRender = t : e.render = t : me(t) && (e.setupState = Ll(t)), dc(e, n)
+function Da(e, t, n) {
+    Q(t) ? e.type.__ssrInlineRender ? e.ssrRender = t : e.render = t : me(t) && (e.setupState = Rl(t)), mc(e, n)
 }
-let Oa;
+let Ia;
 
-function dc(e, t, n) {
+function mc(e, t, n) {
     const r = e.type;
     if (!e.render) {
-        if (!t && Oa && !r.render) {
-            const o = r.template || Hi(e).template;
+        if (!t && Ia && !r.render) {
+            const o = r.template || Ni(e).template;
             if (o) {
                 const {
                     isCustomElement: a,
                     compilerOptions: s
                 } = e.appContext.config, {
                     delimiters: u,
                     compilerOptions: c
                 } = r, l = ye(ye({
                     isCustomElement: a,
                     delimiters: u
                 }, s), c);
-                r.render = Oa(o, l)
+                r.render = Ia(o, l)
             }
         }
         e.render = r.render || mt
     }
-    wn(e), Dn(), ld(e), In(), en()
+    Mn(e), kn(), ld(e), Dn(), en()
 }
 
 function Rd(e) {
     return e.attrsProxy || (e.attrsProxy = new Proxy(e.attrs, {
         get(t, n) {
             return We(e, "get", "$attrs"), t[n]
         }
@@ -3200,45 +3200,45 @@
         },
         slots: e.slots,
         emit: e.emit,
         expose: t
     }
 }
 
-function so(e) {
-    if (e.exposed) return e.exposeProxy || (e.exposeProxy = new Proxy(Ll(Il(e.exposed)), {
+function ao(e) {
+    if (e.exposed) return e.exposeProxy || (e.exposeProxy = new Proxy(Rl(Dl(e.exposed)), {
         get(t, n) {
             if (n in t) return t[n];
-            if (n in Un) return Un[n](e)
+            if (n in Vn) return Vn[n](e)
         },
         has(t, n) {
-            return n in t || n in Un
+            return n in t || n in Vn
         }
     }))
 }
 
 function Bd(e, t = !0) {
     return Q(e) ? e.displayName || e.name : e.name || t && e.__name
 }
 
 function Nd(e) {
     return Q(e) && "__vccOpts" in e
 }
-const re = (e, t) => Gm(e, t, rr);
+const re = (e, t) => Gm(e, t, nr);
 
 function rn(e, t, n) {
     const r = arguments.length;
-    return r === 2 ? me(t) && !K(t) ? xr(t) ? fe(e, null, [t]) : fe(e, t) : fe(e, null, t) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : r === 3 && xr(n) && (n = [n]), fe(e, t, n))
+    return r === 2 ? me(t) && !K(t) ? Hr(t) ? fe(e, null, [t]) : fe(e, t) : fe(e, null, t) : (r > 3 ? n = Array.prototype.slice.call(arguments, 2) : r === 3 && Hr(n) && (n = [n]), fe(e, t, n))
 }
 const Hd = Symbol.for("v-scx"),
     xd = () => ke(Hd),
     Fd = "3.3.4",
     Vd = "http://www.w3.org/2000/svg",
     $t = typeof document < "u" ? document : null,
-    Ga = $t && $t.createElement("template"),
+    Oa = $t && $t.createElement("template"),
     Ud = {
         insert: (e, t, n) => {
             t.insertBefore(e, n || null)
         },
         remove: e => {
             const t = e.parentNode;
             t && t.removeChild(e)
@@ -3264,16 +3264,16 @@
             e.setAttribute(t, "")
         },
         insertStaticContent(e, t, n, r, o, a) {
             const s = n ? n.previousSibling : t.lastChild;
             if (o && (o === a || o.nextSibling))
                 for (; t.insertBefore(o.cloneNode(!0), n), !(o === a || !(o = o.nextSibling)););
             else {
-                Ga.innerHTML = r ? `<svg>${e}</svg>` : e;
-                const u = Ga.content;
+                Oa.innerHTML = r ? `<svg>${e}</svg>` : e;
+                const u = Oa.content;
                 if (r) {
                     const c = u.firstChild;
                     for (; c.firstChild;) u.appendChild(c.firstChild);
                     u.removeChild(c)
                 }
                 t.insertBefore(u, n)
             }
@@ -3287,53 +3287,53 @@
 }
 
 function jd(e, t, n) {
     const r = e.style,
         o = be(n);
     if (n && !o) {
         if (t && !be(t))
-            for (const a in t) n[a] == null && Xo(r, a, "");
-        for (const a in n) Xo(r, a, n[a])
+            for (const a in t) n[a] == null && Ko(r, a, "");
+        for (const a in n) Ko(r, a, n[a])
     } else {
         const a = r.display;
         o ? t !== n && (r.cssText = n) : t && e.removeAttribute("style"), "_vod" in e && (r.display = a)
     }
 }
-const Ra = /\s*!important$/;
+const Ga = /\s*!important$/;
 
-function Xo(e, t, n) {
-    if (K(n)) n.forEach(r => Xo(e, t, r));
+function Ko(e, t, n) {
+    if (K(n)) n.forEach(r => Ko(e, t, r));
     else if (n == null && (n = ""), t.startsWith("--")) e.setProperty(t, n);
     else {
         const r = qd(e, t);
-        Ra.test(n) ? e.setProperty(nn(r), n.replace(Ra, ""), "important") : e[r] = n
+        Ga.test(n) ? e.setProperty(nn(r), n.replace(Ga, ""), "important") : e[r] = n
     }
 }
-const La = ["Webkit", "Moz", "ms"],
-    Po = {};
+const Ra = ["Webkit", "Moz", "ms"],
+    Ao = {};
 
 function qd(e, t) {
-    const n = Po[t];
+    const n = Ao[t];
     if (n) return n;
     let r = gt(t);
-    if (r !== "filter" && r in e) return Po[t] = r;
-    r = ur(r);
-    for (let o = 0; o < La.length; o++) {
-        const a = La[o] + r;
-        if (a in e) return Po[t] = a
+    if (r !== "filter" && r in e) return Ao[t] = r;
+    r = cr(r);
+    for (let o = 0; o < Ra.length; o++) {
+        const a = Ra[o] + r;
+        if (a in e) return Ao[t] = a
     }
     return t
 }
-const Ba = "http://www.w3.org/1999/xlink";
+const La = "http://www.w3.org/1999/xlink";
 
 function Kd(e, t, n, r, o) {
-    if (r && t.startsWith("xlink:")) n == null ? e.removeAttributeNS(Ba, t.slice(6, t.length)) : e.setAttributeNS(Ba, t, n);
+    if (r && t.startsWith("xlink:")) n == null ? e.removeAttributeNS(La, t.slice(6, t.length)) : e.setAttributeNS(La, t, n);
     else {
         const a = Zu(t);
-        n == null || a && !pl(n) ? e.removeAttribute(t) : e.setAttribute(t, a ? "" : n)
+        n == null || a && !_l(n) ? e.removeAttribute(t) : e.setAttribute(t, a ? "" : n)
     }
 }
 
 function Xd(e, t, n, r, o, a, s) {
     if (t === "innerHTML" || t === "textContent") {
         r && s(r, o, a), e[t] = n ?? "";
         return
@@ -3345,15 +3345,15 @@
             d = n ?? "";
         l !== d && (e.value = d), n == null && e.removeAttribute(t);
         return
     }
     let c = !1;
     if (n === "" || n == null) {
         const l = typeof e[t];
-        l === "boolean" ? n = pl(n) : n == null && l === "string" ? (n = "", c = !0) : l === "number" && (n = 0, c = !0)
+        l === "boolean" ? n = _l(n) : n == null && l === "string" ? (n = "", c = !0) : l === "number" && (n = 0, c = !0)
     }
     try {
         e[t] = n
     } catch {}
     c && e.removeAttribute(t)
 }
 
@@ -3373,28 +3373,28 @@
         const [u, c] = Zd(t);
         if (r) {
             const l = a[t] = tf(r, o);
             $d(e, u, l, c)
         } else s && (Yd(e, u, s, c), a[t] = void 0)
     }
 }
-const Na = /(?:Once|Passive|Capture)$/;
+const Ba = /(?:Once|Passive|Capture)$/;
 
 function Zd(e) {
     let t;
-    if (Na.test(e)) {
+    if (Ba.test(e)) {
         t = {};
         let r;
-        for (; r = e.match(Na);) e = e.slice(0, e.length - r[0].length), t[r[0].toLowerCase()] = !0
+        for (; r = e.match(Ba);) e = e.slice(0, e.length - r[0].length), t[r[0].toLowerCase()] = !0
     }
     return [e[2] === ":" ? e.slice(3) : nn(e.slice(2)), t]
 }
-let Eo = 0;
+let Po = 0;
 const Jd = Promise.resolve(),
-    ef = () => Eo || (Jd.then(() => Eo = 0), Eo = Date.now());
+    ef = () => Po || (Jd.then(() => Po = 0), Po = Date.now());
 
 function tf(e, t) {
     const n = r => {
         if (!r._vts) r._vts = Date.now();
         else if (r._vts <= n.attached) return;
         tt(nf(r, n.value), t, 5, [r])
     };
@@ -3405,29 +3405,29 @@
     if (K(t)) {
         const n = e.stopImmediatePropagation;
         return e.stopImmediatePropagation = () => {
             n.call(e), e._stopped = !0
         }, t.map(r => o => !o._stopped && r && r(o))
     } else return t
 }
-const Ha = /^on[a-z]/,
+const Na = /^on[a-z]/,
     rf = (e, t, n, r, o = !1, a, s, u, c) => {
-        t === "class" ? Wd(e, r, o) : t === "style" ? jd(e, n, r) : Xr(t) ? zi(t) || Qd(e, t, n, r, s) : (t[0] === "." ? (t = t.slice(1), !0) : t[0] === "^" ? (t = t.slice(1), !1) : of(e, t, r, o)) ? Xd(e, t, r, a, s, u, c) : (t === "true-value" ? e._trueValue = r : t === "false-value" && (e._falseValue = r), Kd(e, t, r, o))
+        t === "class" ? Wd(e, r, o) : t === "style" ? jd(e, n, r) : Kr(t) ? hi(t) || Qd(e, t, n, r, s) : (t[0] === "." ? (t = t.slice(1), !0) : t[0] === "^" ? (t = t.slice(1), !1) : of(e, t, r, o)) ? Xd(e, t, r, a, s, u, c) : (t === "true-value" ? e._trueValue = r : t === "false-value" && (e._falseValue = r), Kd(e, t, r, o))
     };
 
 function of(e, t, n, r) {
-    return r ? !!(t === "innerHTML" || t === "textContent" || t in e && Ha.test(t) && Q(n)) : t === "spellcheck" || t === "draggable" || t === "translate" || t === "form" || t === "list" && e.tagName === "INPUT" || t === "type" && e.tagName === "TEXTAREA" || Ha.test(t) && be(n) ? !1 : t in e
+    return r ? !!(t === "innerHTML" || t === "textContent" || t in e && Na.test(t) && Q(n)) : t === "spellcheck" || t === "draggable" || t === "translate" || t === "form" || t === "list" && e.tagName === "INPUT" || t === "type" && e.tagName === "TEXTAREA" || Na.test(t) && be(n) ? !1 : t in e
 }
 const Ct = "transition",
-    Rn = "animation",
-    fc = (e, {
+    Gn = "animation",
+    dc = (e, {
         slots: t
-    }) => rn($m, pc(e), t);
-fc.displayName = "Transition";
-const _c = {
+    }) => rn($m, _c(e), t);
+dc.displayName = "Transition";
+const fc = {
         name: String,
         type: String,
         css: {
             type: Boolean,
             default: !0
         },
         duration: [String, Number, Object],
@@ -3437,23 +3437,23 @@
         appearFromClass: String,
         appearActiveClass: String,
         appearToClass: String,
         leaveFromClass: String,
         leaveActiveClass: String,
         leaveToClass: String
     },
-    af = fc.props = ye({}, ql, _c),
+    af = dc.props = ye({}, jl, fc),
     Wt = (e, t = []) => {
         K(e) ? e.forEach(n => n(...t)) : e && e(...t)
     },
-    xa = e => e ? K(e) ? e.some(t => t.length > 1) : e.length > 1 : !1;
+    Ha = e => e ? K(e) ? e.some(t => t.length > 1) : e.length > 1 : !1;
 
-function pc(e) {
+function _c(e) {
     const t = {};
-    for (const x in e) x in _c || (t[x] = e[x]);
+    for (const x in e) x in fc || (t[x] = e[x]);
     if (e.css === !1) return t;
     const {
         name: n = "v",
         type: r,
         duration: o,
         enterFromClass: a = `${n}-enter-from`,
         enterActiveClass: s = `${n}-enter-active`,
@@ -3476,32 +3476,32 @@
     } = t, X = (x, te, De) => {
         Dt(x, te ? d : u), Dt(x, te ? l : s), De && De()
     }, $ = (x, te) => {
         x._isLeaving = !1, Dt(x, m), Dt(x, _), Dt(x, f), te && te()
     }, Y = x => (te, De) => {
         const ot = x ? j : A,
             _e = () => X(te, x, De);
-        Wt(ot, [te, _e]), Fa(() => {
-            Dt(te, x ? c : a), Tt(te, x ? d : u), xa(ot) || Va(te, r, b, _e)
+        Wt(ot, [te, _e]), xa(() => {
+            Dt(te, x ? c : a), Tt(te, x ? d : u), Ha(ot) || Fa(te, r, b, _e)
         })
     };
     return ye(t, {
         onBeforeEnter(x) {
             Wt(v, [x]), Tt(x, a), Tt(x, s)
         },
         onBeforeAppear(x) {
             Wt(N, [x]), Tt(x, c), Tt(x, l)
         },
         onEnter: Y(!1),
         onAppear: Y(!0),
         onLeave(x, te) {
             x._isLeaving = !0;
             const De = () => $(x, te);
-            Tt(x, m), zc(), Tt(x, f), Fa(() => {
-                x._isLeaving && (Dt(x, m), Tt(x, _), xa(P) || Va(x, r, T, De))
+            Tt(x, m), hc(), Tt(x, f), xa(() => {
+                x._isLeaving && (Dt(x, m), Tt(x, _), Ha(P) || Fa(x, r, T, De))
             }), Wt(P, [x, De])
         },
         onEnterCancelled(x) {
             X(x, !1), Wt(I, [x])
         },
         onAppearCancelled(x) {
             X(x, !0), Wt(L, [x])
@@ -3510,21 +3510,21 @@
             $(x), Wt(M, [x])
         }
     })
 }
 
 function sf(e) {
     if (e == null) return null;
-    if (me(e)) return [Mo(e.enter), Mo(e.leave)]; {
-        const t = Mo(e);
+    if (me(e)) return [Eo(e.enter), Eo(e.leave)]; {
+        const t = Eo(e);
         return [t, t]
     }
 }
 
-function Mo(e) {
+function Eo(e) {
     return qu(e)
 }
 
 function Tt(e, t) {
     t.split(/\s+/).forEach(n => n && e.classList.add(n)), (e._vtc || (e._vtc = new Set)).add(t)
 }
 
@@ -3532,143 +3532,143 @@
     t.split(/\s+/).forEach(r => r && e.classList.remove(r));
     const {
         _vtc: n
     } = e;
     n && (n.delete(t), n.size || (e._vtc = void 0))
 }
 
-function Fa(e) {
+function xa(e) {
     requestAnimationFrame(() => {
         requestAnimationFrame(e)
     })
 }
 let lf = 0;
 
-function Va(e, t, n, r) {
+function Fa(e, t, n, r) {
     const o = e._endId = ++lf,
         a = () => {
             o === e._endId && r()
         };
     if (n) return setTimeout(a, n);
     const {
         type: s,
         timeout: u,
         propCount: c
-    } = hc(e, t);
+    } = pc(e, t);
     if (!s) return r();
     const l = s + "end";
     let d = 0;
     const m = () => {
             e.removeEventListener(l, f), a()
         },
         f = _ => {
             _.target === e && ++d >= c && m()
         };
     setTimeout(() => {
         d < c && m()
     }, u + 1), e.addEventListener(l, f)
 }
 
-function hc(e, t) {
+function pc(e, t) {
     const n = window.getComputedStyle(e),
         r = p => (n[p] || "").split(", "),
         o = r(`${Ct}Delay`),
         a = r(`${Ct}Duration`),
-        s = Ua(o, a),
-        u = r(`${Rn}Delay`),
-        c = r(`${Rn}Duration`),
-        l = Ua(u, c);
+        s = Va(o, a),
+        u = r(`${Gn}Delay`),
+        c = r(`${Gn}Duration`),
+        l = Va(u, c);
     let d = null,
         m = 0,
         f = 0;
-    t === Ct ? s > 0 && (d = Ct, m = s, f = a.length) : t === Rn ? l > 0 && (d = Rn, m = l, f = c.length) : (m = Math.max(s, l), d = m > 0 ? s > l ? Ct : Rn : null, f = d ? d === Ct ? a.length : c.length : 0);
+    t === Ct ? s > 0 && (d = Ct, m = s, f = a.length) : t === Gn ? l > 0 && (d = Gn, m = l, f = c.length) : (m = Math.max(s, l), d = m > 0 ? s > l ? Ct : Gn : null, f = d ? d === Ct ? a.length : c.length : 0);
     const _ = d === Ct && /\b(transform|all)(,|$)/.test(r(`${Ct}Property`).toString());
     return {
         type: d,
         timeout: m,
         propCount: f,
         hasTransform: _
     }
 }
 
-function Ua(e, t) {
+function Va(e, t) {
     for (; e.length < t.length;) e = e.concat(e);
-    return Math.max(...t.map((n, r) => Wa(n) + Wa(e[r])))
+    return Math.max(...t.map((n, r) => Ua(n) + Ua(e[r])))
 }
 
-function Wa(e) {
+function Ua(e) {
     return Number(e.slice(0, -1).replace(",", ".")) * 1e3
 }
 
-function zc() {
+function hc() {
     return document.body.offsetHeight
 }
-const bc = new WeakMap,
-    gc = new WeakMap,
-    yc = {
+const zc = new WeakMap,
+    bc = new WeakMap,
+    gc = {
         name: "TransitionGroup",
         props: ye({}, af, {
             tag: String,
             moveClass: String
         }),
         setup(e, {
             slots: t
         }) {
-            const n = On(),
-                r = jl();
+            const n = In(),
+                r = Wl();
             let o, a;
-            return $l(() => {
+            return Xl(() => {
                 if (!o.length) return;
                 const s = e.moveClass || `${e.name||"v"}-move`;
                 if (!ff(o[0].el, n.vnode.el, s)) return;
                 o.forEach(uf), o.forEach(mf);
                 const u = o.filter(df);
-                zc(), u.forEach(c => {
+                hc(), u.forEach(c => {
                     const l = c.el,
                         d = l.style;
                     Tt(l, s), d.transform = d.webkitTransform = d.transitionDuration = "";
                     const m = l._moveCb = f => {
                         f && f.target !== l || (!f || /transform$/.test(f.propertyName)) && (l.removeEventListener("transitionend", m), l._moveCb = null, Dt(l, s))
                     };
                     l.addEventListener("transitionend", m)
                 })
             }), () => {
                 const s = ee(e),
-                    u = pc(s);
+                    u = _c(s);
                 let c = s.tag || He;
-                o = a, a = t.default ? Ri(t.default()) : [];
+                o = a, a = t.default ? Gi(t.default()) : [];
                 for (let l = 0; l < a.length; l++) {
                     const d = a[l];
-                    d.key != null && tr(d, er(d, u, r, n))
+                    d.key != null && er(d, Jn(d, u, r, n))
                 }
                 if (o)
                     for (let l = 0; l < o.length; l++) {
                         const d = o[l];
-                        tr(d, er(d, u, r, n)), bc.set(d, d.el.getBoundingClientRect())
+                        er(d, Jn(d, u, r, n)), zc.set(d, d.el.getBoundingClientRect())
                     }
                 return fe(c, null, a)
             }
         }
     },
     cf = e => delete e.mode;
-yc.props;
-const sb = yc;
+gc.props;
+const sb = gc;
 
 function uf(e) {
     const t = e.el;
     t._moveCb && t._moveCb(), t._enterCb && t._enterCb()
 }
 
 function mf(e) {
-    gc.set(e, e.el.getBoundingClientRect())
+    bc.set(e, e.el.getBoundingClientRect())
 }
 
 function df(e) {
-    const t = bc.get(e),
-        n = gc.get(e),
+    const t = zc.get(e),
+        n = bc.get(e),
         r = t.left - n.left,
         o = t.top - n.top;
     if (r || o) {
         const a = e.el.style;
         return a.transform = a.webkitTransform = `translate(${r}px,${o}px)`, a.transitionDuration = "0s", e
     }
 }
@@ -3678,15 +3678,15 @@
     e._vtc && e._vtc.forEach(s => {
         s.split(/\s+/).forEach(u => u && r.classList.remove(u))
     }), n.split(/\s+/).forEach(s => s && r.classList.add(s)), r.style.display = "none";
     const o = t.nodeType === 1 ? t : t.parentNode;
     o.appendChild(r);
     const {
         hasTransform: a
-    } = hc(r);
+    } = pc(r);
     return o.removeChild(r), a
 }
 const _f = ["ctrl", "shift", "alt", "meta"],
     pf = {
         stop: e => e.stopPropagation(),
         prevent: e => e.preventDefault(),
         self: e => e.target !== e.currentTarget,
@@ -3722,50 +3722,50 @@
     },
     ub = {
         beforeMount(e, {
             value: t
         }, {
             transition: n
         }) {
-            e._vod = e.style.display === "none" ? "" : e.style.display, n && t ? n.beforeEnter(e) : Ln(e, t)
+            e._vod = e.style.display === "none" ? "" : e.style.display, n && t ? n.beforeEnter(e) : Rn(e, t)
         },
         mounted(e, {
             value: t
         }, {
             transition: n
         }) {
             n && t && n.enter(e)
         },
         updated(e, {
             value: t,
             oldValue: n
         }, {
             transition: r
         }) {
-            !t != !n && (r ? t ? (r.beforeEnter(e), Ln(e, !0), r.enter(e)) : r.leave(e, () => {
-                Ln(e, !1)
-            }) : Ln(e, t))
+            !t != !n && (r ? t ? (r.beforeEnter(e), Rn(e, !0), r.enter(e)) : r.leave(e, () => {
+                Rn(e, !1)
+            }) : Rn(e, t))
         },
         beforeUnmount(e, {
             value: t
         }) {
-            Ln(e, t)
+            Rn(e, t)
         }
     };
 
-function Ln(e, t) {
+function Rn(e, t) {
     e.style.display = t ? e._vod : "none"
 }
 const zf = ye({
     patchProp: rf
 }, Ud);
-let ja;
+let Wa;
 
 function bf() {
-    return ja || (ja = yd(zf))
+    return Wa || (Wa = yd(zf))
 }
 const gf = (...e) => {
     const t = bf().createApp(...e),
         {
             mount: n
         } = t;
     return t.mount = r => {
@@ -3802,82 +3802,82 @@
     topBarContextMenuItems: [],
     blockGlobalPlayMenu: !1,
     alwaysShowMenuButton: !1,
     apiInitialized: !1,
     apiBaseUrl: "",
     prevRoutes: []
 });
-var vr = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
+var yr = typeof globalThis < "u" ? globalThis : typeof window < "u" ? window : typeof global < "u" ? global : typeof self < "u" ? self : {};
 
-function vc(e) {
+function yc(e) {
     return e && e.__esModule && Object.prototype.hasOwnProperty.call(e, "default") ? e.default : e
 }
-var $o = {},
-    Tc = {};
-Object.defineProperty(Tc, "__esModule", {
+var Xo = {},
+    vc = {};
+Object.defineProperty(vc, "__esModule", {
     value: !0
 });
-var lo = {};
-Object.defineProperty(lo, "__esModule", {
+var so = {};
+Object.defineProperty(so, "__esModule", {
     value: !0
 });
-lo.ConstantBackoff = void 0;
+so.ConstantBackoff = void 0;
 var vf = function() {
     function e(t) {
         this.reset = function() {}, this.backoff = t
     }
     return e.prototype.next = function() {
         return this.backoff
     }, e
 }();
-lo.ConstantBackoff = vf;
-var co = {};
-Object.defineProperty(co, "__esModule", {
+so.ConstantBackoff = vf;
+var lo = {};
+Object.defineProperty(lo, "__esModule", {
     value: !0
 });
-co.ExponentialBackoff = void 0;
+lo.ExponentialBackoff = void 0;
 var Tf = function() {
     function e(t, n) {
         this.initial = t, this.expMax = n, this.expCurrent = 1, this.current = this.initial
     }
     return e.prototype.next = function() {
         var t = this.current;
         return this.expMax > this.expCurrent++ && (this.current = this.current * 2), t
     }, e.prototype.reset = function() {
         this.expCurrent = 1, this.current = this.initial
     }, e
 }();
-co.ExponentialBackoff = Tf;
-var uo = {};
-Object.defineProperty(uo, "__esModule", {
+lo.ExponentialBackoff = Tf;
+var co = {};
+Object.defineProperty(co, "__esModule", {
     value: !0
 });
-uo.LinearBackoff = void 0;
+co.LinearBackoff = void 0;
 var Sf = function() {
     function e(t, n, r) {
         this.initial = t, this.increment = n, this.maximum = r, this.current = this.initial
     }
     return e.prototype.next = function() {
         var t = this.current,
             n = this.current + this.increment;
         return this.maximum === void 0 ? this.current = n : n <= this.maximum && (this.current = n), t
     }, e.prototype.reset = function() {
         this.current = this.initial
     }, e
 }();
-uo.LinearBackoff = Sf;
-var Sc = {};
-Object.defineProperty(Sc, "__esModule", {
+co.LinearBackoff = Sf;
+var Tc = {};
+Object.defineProperty(Tc, "__esModule", {
     value: !0
 });
-var mo = {};
-Object.defineProperty(mo, "__esModule", {
+var uo = {};
+Object.defineProperty(uo, "__esModule", {
     value: !0
 });
-mo.LRUBuffer = void 0;
+uo.LRUBuffer = void 0;
 var Af = function() {
     function e(t) {
         this.writePtr = 0, this.wrapped = !1, this.buffer = Array(t)
     }
     return e.prototype.len = function() {
         return this.wrapped ? this.buffer.length : this.writePtr
     }, e.prototype.cap = function() {
@@ -3897,20 +3897,20 @@
         if (this.writePtr === 0 && !this.wrapped) return 0;
         for (var n = this.wrapped ? this.writePtr : 0, r = this.wrapped ? n - 1 < 0 ? this.buffer.length - 1 : n - 1 : this.writePtr - 1, o = this.len(); t(this.buffer[n]), n !== r;) n = (n + 1) % this.buffer.length;
         return o
     }, e.prototype.clear = function() {
         this.writePtr = 0, this.wrapped = !1
     }, e
 }();
-mo.LRUBuffer = Af;
-var fo = {};
-Object.defineProperty(fo, "__esModule", {
+uo.LRUBuffer = Af;
+var mo = {};
+Object.defineProperty(mo, "__esModule", {
     value: !0
 });
-fo.TimeBuffer = void 0;
+mo.TimeBuffer = void 0;
 var Pf = function() {
     function e(t) {
         this.maxAge = t
     }
     return e.prototype.cap = function() {
         return Number.POSITIVE_INFINITY
     }, e.prototype.len = function() {
@@ -3936,16 +3936,16 @@
         };
         this.tail === void 0 && (this.tail = n), this.head === void 0 ? this.head = n : (this.head.n = n, this.head = n)
     }, e.prototype.forwardTail = function() {
         if (this.tail !== void 0)
             for (var t = Date.now(); t - this.tail.t > this.maxAge && (this.tail === this.head ? (this.tail = void 0, this.head = void 0) : this.tail = this.tail.n, this.tail !== void 0););
     }, e.prototype.clear = function() {}, e
 }();
-fo.TimeBuffer = Pf;
-var qi = {};
+mo.TimeBuffer = Pf;
+var ji = {};
 (function(e) {
     Object.defineProperty(e, "__esModule", {
         value: !0
     }), e.Websocket = e.WebsocketEvents = void 0;
     var t;
     (function(r) {
         r.open = "open", r.close = "close", r.error = "error", r.message = "message", r.retry = "retry"
@@ -4026,21 +4026,21 @@
                         }
                     })), o.tryConnect()
                 }, a)
             }
         }, r
     }();
     e.Websocket = n
-})(qi);
-var _o = {};
-Object.defineProperty(_o, "__esModule", {
+})(ji);
+var fo = {};
+Object.defineProperty(fo, "__esModule", {
     value: !0
 });
-_o.WebsocketBuilder = void 0;
-var cn = qi,
+fo.WebsocketBuilder = void 0;
+var cn = ji,
     Ef = function() {
         function e(t) {
             this.ws = null, this.onOpenListeners = [], this.onCloseListeners = [], this.onErrorListeners = [], this.onMessageListeners = [], this.onRetryListeners = [], this.url = t
         }
         return e.prototype.withProtocols = function(t) {
             return this.protocols = t, this
         }, e.prototype.withBackoff = function(t) {
@@ -4088,37 +4088,37 @@
                 return (r = t.ws) === null || r === void 0 ? void 0 : r.addEventListener(cn.WebsocketEvents.message, n.listener, n.options)
             }), this.onRetryListeners.forEach(function(n) {
                 var r;
                 return (r = t.ws) === null || r === void 0 ? void 0 : r.addEventListener(cn.WebsocketEvents.retry, n.listener, n.options)
             }), this.ws)
         }, e
     }();
-_o.WebsocketBuilder = Ef;
+fo.WebsocketBuilder = Ef;
 (function(e) {
-    var t = vr && vr.__createBinding || (Object.create ? function(r, o, a, s) {
+    var t = yr && yr.__createBinding || (Object.create ? function(r, o, a, s) {
             s === void 0 && (s = a), Object.defineProperty(r, s, {
                 enumerable: !0,
                 get: function() {
                     return o[a]
                 }
             })
         } : function(r, o, a, s) {
             s === void 0 && (s = a), r[s] = o[a]
         }),
-        n = vr && vr.__exportStar || function(r, o) {
+        n = yr && yr.__exportStar || function(r, o) {
             for (var a in r) a !== "default" && !Object.prototype.hasOwnProperty.call(o, a) && t(o, r, a)
         };
     Object.defineProperty(e, "__esModule", {
         value: !0
-    }), n(Tc, e), n(lo, e), n(co, e), n(uo, e), n(Sc, e), n(mo, e), n(fo, e), n(qi, e), n(_o, e)
-})($o);
+    }), n(vc, e), n(so, e), n(lo, e), n(co, e), n(Tc, e), n(uo, e), n(mo, e), n(ji, e), n(fo, e)
+})(Xo);
 const Mf = 1,
-    Fr = 2,
-    wo = 3,
-    Ki = 4,
+    xr = 2,
+    Mo = 3,
+    qi = 4,
     wf = 5,
     Cf = 6;
 
 function kf(e) {
     return {
         type: "auth",
         access_token: e
@@ -4138,15 +4138,15 @@
 function If(e) {
     const t = {
         type: "subscribe_events"
     };
     return e && (t.event_type = e), t
 }
 
-function qa(e) {
+function ja(e) {
     return {
         type: "unsubscribe_events",
         subscription: e
     }
 }
 
 function Of() {
@@ -4181,43 +4181,43 @@
         const [o, a, s] = e.split(".", 3);
         return Number(o) > t || Number(o) === t && (r === void 0 ? Number(a) >= n : Number(a) > n) || r !== void 0 && Number(o) === t && Number(a) === n && Number(s) >= r
     },
     Bf = "auth_invalid",
     Nf = "auth_ok";
 
 function Hf(e) {
-    if (!e.auth) throw Ki;
+    if (!e.auth) throw qi;
     const t = e.auth;
     let n = t.expired ? t.refreshAccessToken().then(() => {
         n = void 0
     }, () => {
         n = void 0
     }) : void 0;
     const r = t.wsUrl;
 
     function o(a, s, u) {
         const c = new WebSocket(r);
         let l = !1;
         const d = () => {
                 if (c.removeEventListener("close", d), l) {
-                    u(Fr);
+                    u(xr);
                     return
                 }
                 if (a === 0) {
                     u(Mf);
                     return
                 }
                 const _ = a === -1 ? -1 : a - 1;
                 setTimeout(() => o(_, s, u), 1e3)
             },
             m = async _ => {
                 try {
                     t.expired && await (n || t.refreshAccessToken()), c.send(JSON.stringify(kf(t.accessToken)))
                 } catch (p) {
-                    l = p === Fr, c.close()
+                    l = p === xr, c.close()
                 }
             }, f = async _ => {
                 const p = JSON.parse(_.data);
                 switch (p.type) {
                     case Bf:
                         l = !0, c.close();
                         break;
@@ -4234,45 +4234,45 @@
     constructor(t, n) {
         this._handleMessage = r => {
             let o = JSON.parse(r.data);
             Array.isArray(o) || (o = [o]), o.forEach(a => {
                 const s = this.commands.get(a.id);
                 switch (a.type) {
                     case "event":
-                        s ? s.callback(a.event) : (console.warn(`Received event for unknown subscription ${a.id}. Unsubscribing.`), this.sendMessagePromise(qa(a.id)));
+                        s ? s.callback(a.event) : (console.warn(`Received event for unknown subscription ${a.id}. Unsubscribing.`), this.sendMessagePromise(ja(a.id)));
                         break;
                     case "result":
                         s && (a.success ? (s.resolve(a.result), "subscribe" in s || this.commands.delete(a.id)) : (s.reject(a.error), this.commands.delete(a.id)));
                         break;
                     case "pong":
                         s ? (s.resolve(), this.commands.delete(a.id)) : console.warn(`Received unknown pong response ${a.id}`);
                         break
                 }
             })
         }, this._handleClose = async () => {
             const r = this.commands;
             if (this.commandId = 1, this.oldSubscriptions = this.commands, this.commands = new Map, this.socket = void 0, r.forEach(s => {
-                    "subscribe" in s || s.reject(Gf(wo, "Connection lost"))
+                    "subscribe" in s || s.reject(Gf(Mo, "Connection lost"))
                 }), this.closeRequested) return;
             this.fireEvent("disconnected");
             const o = Object.assign(Object.assign({}, this.options), {
                     setupRetry: 0
                 }),
                 a = s => {
                     setTimeout(async () => {
                         if (!this.closeRequested) try {
                             const u = await o.createSocket(o);
                             this._setSocket(u)
                         } catch (u) {
                             if (this._queuedMessages) {
                                 const c = this._queuedMessages;
                                 this._queuedMessages = void 0;
-                                for (const l of c) l.reject && l.reject(wo)
+                                for (const l of c) l.reject && l.reject(Mo)
                             }
-                            u === Fr ? this.fireEvent("reconnect-error", u) : a(s + 1)
+                            u === xr ? this.fireEvent("reconnect-error", u) : a(s + 1)
                         }
                     }, Math.min(s, 5) * 1e3)
                 };
             this.suspendReconnectPromise && (await this.suspendReconnectPromise, this.suspendReconnectPromise = void 0, this._queuedMessages = []), a(0)
         }, this.options = n, this.commandId = 2, this.commands = new Map, this.eventListeners = new Map, this.closeRequested = !1, this._setSocket(t)
     }
     get connected() {
@@ -4328,15 +4328,15 @@
     async subscribeEvents(t, n) {
         return this.subscribeMessage(t, If(n))
     }
     ping() {
         return this.sendMessagePromise(Of())
     }
     sendMessage(t, n) {
-        if (!this.connected) throw wo;
+        if (!this.connected) throw Mo;
         if (this._queuedMessages) {
             if (n) throw new Error("Cannot queue with commandId");
             this._queuedMessages.push({
                 resolve: () => this.sendMessage(t)
             });
             return
         }
@@ -4376,15 +4376,15 @@
             const u = this._genCmdId();
             o = {
                 resolve: a,
                 reject: s,
                 callback: t,
                 subscribe: (r == null ? void 0 : r.resubscribe) !== !1 ? () => this.subscribeMessage(t, n) : void 0,
                 unsubscribe: async () => {
-                    this.connected && await this.sendMessagePromise(qa(u)), this.commands.delete(u)
+                    this.connected && await this.sendMessagePromise(ja(u)), this.commands.delete(u)
                 }
             }, this.commands.set(u, o);
             try {
                 this.sendMessage(n, u)
             } catch {}
         }), () => o.unsubscribe()
     }
@@ -4409,36 +4409,36 @@
     let o = `${e}/auth/authorize?response_type=code&redirect_uri=${encodeURIComponent(n)}`;
     return t !== null && (o += `&client_id=${encodeURIComponent(t)}`), r && (o += `&state=${encodeURIComponent(r)}`), o
 }
 
 function jf(e, t, n, r) {
     n += (n.includes("?") ? "&" : "?") + "auth_callback=1", document.location.href = Wf(e, t, n, r)
 }
-async function Ac(e, t, n) {
+async function Sc(e, t, n) {
     const r = typeof location < "u" && location;
     if (r && r.protocol === "https:") {
         const u = document.createElement("a");
         if (u.href = e, u.protocol === "http:" && u.hostname !== "localhost") throw wf
     }
     const o = new FormData;
     t !== null && o.append("client_id", t), Object.keys(n).forEach(u => {
         o.append(u, n[u])
     });
     const a = await fetch(`${e}/auth/token`, {
         method: "POST",
         credentials: "same-origin",
         body: o
     });
-    if (!a.ok) throw a.status === 400 || a.status === 403 ? Fr : new Error("Unable to fetch tokens");
+    if (!a.ok) throw a.status === 400 || a.status === 403 ? xr : new Error("Unable to fetch tokens");
     const s = await a.json();
     return s.hassUrl = e, s.clientId = t, s.expires = Vf(s.expires_in), s
 }
 
-function Ka(e, t, n) {
-    return Ac(e, t, {
+function qa(e, t, n) {
+    return Sc(e, t, {
         code: n,
         grant_type: "authorization_code"
     })
 }
 
 function qf(e) {
     return btoa(JSON.stringify(e))
@@ -4458,15 +4458,15 @@
         return this.data.access_token
     }
     get expired() {
         return Date.now() > this.data.expires
     }
     async refreshAccessToken() {
         if (!this.data.refresh_token) throw new Error("No refresh_token");
-        const t = await Ac(this.data.hassUrl, this.data.clientId, {
+        const t = await Sc(this.data.hassUrl, this.data.clientId, {
             grant_type: "refresh_token",
             refresh_token: this.data.refresh_token
         });
         t.refresh_token = this.data.refresh_token, this.data = t, this._saveTokens && this._saveTokens(t)
     }
     async revoke() {
         if (!this.data.refresh_token) throw new Error("No refresh_token to revoke");
@@ -4474,29 +4474,29 @@
         t.append("token", this.data.refresh_token), await fetch(`${this.data.hassUrl}/auth/revoke`, {
             method: "POST",
             credentials: "same-origin",
             body: t
         }), this._saveTokens && this._saveTokens(null)
     }
 }
-async function Xa(e = {}) {
+async function Ka(e = {}) {
     let t, n = e.hassUrl;
     n && n[n.length - 1] === "/" && (n = n.substr(0, n.length - 1));
     const r = e.clientId !== void 0 ? e.clientId : Ff(),
         o = e.limitHassInstance === !0;
-    if (e.authCode && n && (t = await Ka(n, r, e.authCode), e.saveTokens && e.saveTokens(t)), !t) {
+    if (e.authCode && n && (t = await qa(n, r, e.authCode), e.saveTokens && e.saveTokens(t)), !t) {
         const a = Rf(location.search.substr(1));
         if ("auth_callback" in a) {
             const s = Kf(a.state);
             if (o && (s.hassUrl !== n || s.clientId !== r)) throw Cf;
-            t = await Ka(s.hassUrl, s.clientId, a.code), e.saveTokens && e.saveTokens(t)
+            t = await qa(s.hassUrl, s.clientId, a.code), e.saveTokens && e.saveTokens(t)
         }
     }
     if (!t && e.loadTokens && (t = await e.loadTokens()), t) return new Xf(t, e.saveTokens);
-    if (n === void 0) throw Ki;
+    if (n === void 0) throw qi;
     return jf(n, r, e.redirectUrl || Uf(), qf({
         hassUrl: n,
         clientId: r
     })), new Promise(() => {})
 }
 async function $f(e) {
     const t = Object.assign({
@@ -4506,16 +4506,16 @@
         n = await t.createSocket(t);
     return new xf(n, t)
 }
 const mb = "this_value_is_encrypted";
 var Yf = (e => (e.ARTIST = "artist", e.ALBUM = "album", e.TRACK = "track", e.PLAYLIST = "playlist", e.RADIO = "radio", e.FOLDER = "folder", e.UNKNOWN = "unknown", e))(Yf || {}),
     Qf = (e => (e.THUMB = "thumb", e.WIDE_THUMB = "wide_thumb", e.FANART = "fanart", e.LOGO = "logo", e.CLEARART = "clearart", e.BANNER = "banner", e.CUTOUT = "cutout", e.BACK = "back", e.CDART = "cdart", e.EMBEDDED_THUMB = "embedded_thumb", e.OTHER = "other", e))(Qf || {}),
     Zf = (e => (e.OGG = "ogg", e.FLAC = "flac", e.MP3 = "mp3", e.AAC = "aac", e.MPEG = "mpeg", e.ALAC = "alac", e.WAV = "wav", e.AIFF = "aiff", e.WMA = "wma", e.M4B = "m4b", e.M4A = "m4a", e.DSF = "dsf", e.WAVPACK = "wv", e.PCM_S16LE = "s16le", e.PCM_S24LE = "s24le", e.PCM_S32LE = "s32le", e.PCM_F32LE = "f32le", e.PCM_F64LE = "f64le", e.MPEG_DASH = "dash", e.UNKNOWN = "?", e))(Zf || {}),
-    fn = (e => (e.PLAY = "play", e.REPLACE = "replace", e.NEXT = "next", e.REPLACE_NEXT = "replace_next", e.ADD = "add", e))(fn || {}),
-    _n = (e => (e.OFF = "off", e.ONE = "one", e.ALL = "all", e))(_n || {}),
+    Ac = (e => (e.PLAY = "play", e.REPLACE = "replace", e.NEXT = "next", e.REPLACE_NEXT = "replace_next", e.ADD = "add", e))(Ac || {}),
+    fn = (e => (e.OFF = "off", e.ONE = "one", e.ALL = "all", e))(fn || {}),
     Jf = (e => (e.IDLE = "idle", e.PAUSED = "paused", e.PLAYING = "playing", e))(Jf || {}),
     Pc = (e => (e.PLAYER = "player", e.GROUP = "group", e.STEREO_PAIR = "stereo_pair", e))(Pc || {}),
     at = (e => (e.PLAYER_ADDED = "player_added", e.PLAYER_UPDATED = "player_updated", e.PLAYER_REMOVED = "player_removed", e.PLAYER_SETTINGS_UPDATED = "player_settings_updated", e.QUEUE_ADDED = "queue_added", e.QUEUE_UPDATED = "queue_updated", e.QUEUE_ITEMS_UPDATED = "queue_items_updated", e.QUEUE_TIME_UPDATED = "queue_time_updated", e.QUEUE_SETTINGS_UPDATED = "queue_settings_updated", e.SHUTDOWN = "application_shutdown", e.MEDIA_ITEM_ADDED = "media_item_added", e.MEDIA_ITEM_UPDATED = "media_item_updated", e.MEDIA_ITEM_DELETED = "media_item_deleted", e.PROVIDERS_UPDATED = "providers_updated", e.PLAYER_CONFIG_UPDATED = "player_config_updated", e.SYNC_TASKS_UPDATED = "sync_tasks_updated", e.AUTH_SESSION = "auth_session", e.ALL = "*", e))(at || {}),
     e_ = (e => (e.BROWSE = "browse", e.SEARCH = "search", e.RECOMMENDATIONS = "recommendations", e.LIBRARY_ARTISTS = "library_artists", e.LIBRARY_ALBUMS = "library_albums", e.LIBRARY_TRACKS = "library_tracks", e.LIBRARY_PLAYLISTS = "library_playlists", e.LIBRARY_RADIOS = "library_radios", e.ARTIST_ALBUMS = "artist_albums", e.ARTIST_TOPTRACKS = "artist_toptracks", e.LIBRARY_ARTISTS_EDIT = "library_artists_edit", e.LIBRARY_ALBUMS_EDIT = "library_albums_edit", e.LIBRARY_TRACKS_EDIT = "library_tracks_edit", e.LIBRARY_PLAYLISTS_EDIT = "library_playlists_edit", e.LIBRARY_RADIOS_EDIT = "library_radios_edit", e.SIMILAR_TRACKS = "similar_tracks", e.PLAYLIST_TRACKS_EDIT = "playlist_tracks_edit", e.PLAYLIST_CREATE = "playlist_create", e.CREATE_GROUP = "create_group", e.DELETE_GROUP = "delete_group", e))(e_ || {}),
     t_ = (e => (e.MUSIC = "music", e.PLAYER = "player", e.METADATA = "metadata", e.PLUGIN = "plugin", e))(t_ || {}),
     n_ = (e => (e.BOOLEAN = "boolean", e.STRING = "string", e.SECURE_STRING = "secure_string", e.INTEGER = "integer", e.FLOAT = "float", e.LABEL = "label", e.DIVIDER = "divider", e.ACTION = "action", e))(n_ || {}),
     r_ = (e => (e[e.DISCONNECTED = 0] = "DISCONNECTED", e[e.CONNECTING = 1] = "CONNECTING", e[e.CONNECTED = 2] = "CONNECTED", e))(r_ || {});
@@ -4537,26 +4537,26 @@
         Be(this, "commands");
         this.commandId = 0, this.eventCallbacks = [], this.commands = new Map
     }
     async initialize(t) {
         if (this.ws) throw new Error("already initialized");
         t.endsWith("/") && (t = t.slice(0, -1)), this.baseUrl = t;
         const n = t.replace("http", "ws") + "/ws";
-        console.log(`Connecting to Music Assistant API ${n}`), this.state.value = 1, this.ws = new $o.WebsocketBuilder(n).onOpen((r, o) => {
+        console.log(`Connecting to Music Assistant API ${n}`), this.state.value = 1, this.ws = new Xo.WebsocketBuilder(n).onOpen((r, o) => {
             console.log("connection opened")
         }).onClose((r, o) => {
             console.log("connection closed"), this.state.value = 0
         }).onError((r, o) => {
             console.log("error on connection")
         }).onMessage((r, o) => {
             const a = JSON.parse(o.data);
             "event" in a ? this.handleEventMessage(a) : "server_version" in a ? this.handleServerInfoMessage(a) : "message_id" in a && "is_last_chunk" in a ? this.handleChunkedResultMessage(a) : "message_id" in a ? this.handleResultMessage(a) : console.error("received unknown message", a)
         }).onRetry((r, o) => {
             console.log("retry"), this.state.value = 1
-        }).withBackoff(new $o.LinearBackoff(0, 1e3, 12e3)).build()
+        }).withBackoff(new Xo.LinearBackoff(0, 1e3, 12e3)).build()
     }
     subscribe(t, n) {
         const r = [t, n];
         return this.eventCallbacks.push(r), () => {
             const a = this.eventCallbacks.indexOf(r);
             a > -1 && this.eventCallbacks.splice(a, 1)
         }
@@ -4594,15 +4594,15 @@
         return this.getData("music/tracks/track_albums", {
             item_id: t,
             provider_instance_id_or_domain: n
         })
     }
     getTrackPreviewUrl(t, n) {
         const r = encodeURIComponent(encodeURIComponent(n));
-        return `${Yo.baseUrl}/preview?item_id=${r}&provider=${t}`
+        return `${$o.baseUrl}/preview?item_id=${r}&provider=${t}`
     }
     getLibraryArtists(t, n, r, o, a, s) {
         return this.getData("music/artists/library_items", {
             favorite: t,
             search: n,
             limit: r,
             offset: o,
@@ -4700,15 +4700,15 @@
             search: n,
             limit: r,
             offset: o,
             order_by: a
         })
     }
     getRadio(t, n, r, o) {
-        return this.getData("music/radios/get_radio", {
+        return this.getData("music/radio/get_radio", {
             item_id: t,
             provider_instance_id_or_domain: n,
             force_refresh: r,
             lazy: o
         })
     }
     getRadioVersions(t, n) {
@@ -4859,15 +4859,15 @@
             crossfade_enabled: n
         })
     }
     queueCommandCrossfadeToggle(t) {
         this.queueCommandCrossfade(t, !this.queues[t].crossfade_enabled)
     }
     queueCommandRepeatToggle(t) {
-        this.queues[t], this.queues[t].repeat_mode == _n.OFF ? this.queueCommandRepeat(t, _n.ONE) : this.queues[t].repeat_mode == _n.ONE ? this.queueCommandRepeat(t, _n.ALL) : this.queueCommandRepeat(t, _n.OFF)
+        this.queues[t], this.queues[t].repeat_mode == fn.OFF ? this.queueCommandRepeat(t, fn.ONE) : this.queues[t].repeat_mode == fn.ONE ? this.queueCommandRepeat(t, fn.ALL) : this.queueCommandRepeat(t, fn.OFF)
     }
     playerQueueCommand(t, n, r) {
         clearTimeout(this._throttleId), this._throttleId = setTimeout(() => {
             this.sendCommand(`players/queue/${n}`, {
                 queue_id: t,
                 ...r
             })
@@ -4926,34 +4926,24 @@
     }
     setPlayerGroupMembers(t, n) {
         this.sendCommand("players/cmd/set_members", {
             player_id: t,
             members: n
         })
     }
-    playMedia(t, n = fn.PLAY, r, o) {
-        var a, s, u;
-        !o && ut.selectedPlayer && ((a = ut.selectedPlayer) == null ? void 0 : a.active_source) in this.players ? o = (s = ut.selectedPlayer) == null ? void 0 : s.active_source : o || (o = (u = ut.selectedPlayer) == null ? void 0 : u.player_id), this.sendCommand("players/queue/play_media", {
-            queue_id: o,
+    playMedia(t, n = Ac.PLAY, r, o, a) {
+        var s, u, c;
+        !a && ut.selectedPlayer && ((s = ut.selectedPlayer) == null ? void 0 : s.active_source) in this.players ? a = (u = ut.selectedPlayer) == null ? void 0 : u.active_source : a || (a = (c = ut.selectedPlayer) == null ? void 0 : c.player_id), this.sendCommand("players/queue/play_media", {
+            queue_id: a,
             media: t,
             option: n,
-            radio_mode: r
+            radio_mode: r,
+            start_item: o
         })
     }
-    async playPlaylistFromIndex(t, n, r) {
-        const o = await this.getPlaylistTracks(t.item_id, t.provider);
-        this.playMedia(o[n], fn.REPLACE, void 0, r), this.playMedia(o.slice(n + 1), fn.ADD, void 0, r)
-    }
-    async playAlbumFromItem(t, n, r) {
-        const o = await this.getAlbumTracks(t.item_id, t.provider);
-        let a = 0;
-        o.forEach(function(s, u) {
-            s.item_id == n.item_id && (a = u)
-        }), this.playMedia(o[a], fn.REPLACE, void 0, r), this.playMedia(o.slice(a + 1), fn.ADD, void 0, r)
-    }
     async getProviderConfigs(t, n) {
         return this.getData("config/providers", {
             provider_type: t,
             provider_domain: n
         })
     }
     async getProviderConfig(t) {
@@ -5057,19 +5047,19 @@
             },
             saveTokens: o => {
                 localStorage.hassTokens = JSON.stringify(o)
             },
             hassUrl: ""
         };
         try {
-            t = await Xa(n)
+            t = await Ka(n)
         } catch (o) {
-            if (o === Ki) {
+            if (o === qi) {
                 if (n.hassUrl = prompt("Please enter the URL to Home Assistant", "http://homeassistant.local:8123") || "", !n.hassUrl) return;
-                t = await Xa(n)
+                t = await Ka(n)
             } else {
                 alert(`Unknown error: ${o}`);
                 return
             }
         }
         const r = await $f({
             auth: t
@@ -5145,34 +5135,34 @@
         for (const t of await this.getData("providers")) this.providers[t.instance_id] = t;
         this.syncTasks.value = await this.getData("music/synctasks")
     }
     _genCmdId() {
         return ++this.commandId
     }
 }
-const Yo = new o_;
+const $o = new o_;
 
 function Ec(e, t) {
     let n;
 
     function r() {
-        n = bl(), n.run(() => t.length ? t(() => {
+        n = zl(), n.run(() => t.length ? t(() => {
             n == null || n.stop(), r()
         }) : t())
     }
     xe(e, o => {
         o && !n ? r() : o || (n == null || n.stop(), n = void 0)
     }, {
         immediate: !0
     }), tm(() => {
         n == null || n.stop()
     })
 }
 
-function $a(e, t, n) {
+function Xa(e, t, n) {
     i_(e, t), t.set(e, n)
 }
 
 function i_(e, t) {
     if (t.has(e)) throw new TypeError("Cannot initialize the same private elements twice on an object")
 }
 
@@ -5216,26 +5206,26 @@
 function c_(e, t) {
     if (e === t) return !0;
     if (e instanceof Date && t instanceof Date && e.getTime() !== t.getTime() || e !== Object(e) || t !== Object(t)) return !1;
     const n = Object.keys(e);
     return n.length !== Object.keys(t).length ? !1 : n.every(r => c_(e[r], t[r]))
 }
 
-function Qo(e, t, n) {
+function Yo(e, t, n) {
     return e == null || !t || typeof t != "string" ? n : e[t] !== void 0 ? e[t] : (t = t.replace(/\[(\w+)\]/g, ".$1"), t = t.replace(/^\./, ""), wc(e, t.split("."), n))
 }
 
 function db(e, t, n) {
     if (t == null) return e === void 0 ? n : e;
     if (e !== Object(e)) {
         if (typeof t != "function") return n;
         const o = t(e, n);
         return typeof o > "u" ? n : o
     }
-    if (typeof t == "string") return Qo(e, t, n);
+    if (typeof t == "string") return Yo(e, t, n);
     if (Array.isArray(t)) return wc(e, t, n);
     if (typeof t != "function") return n;
     const r = t(e, n);
     return typeof r > "u" ? n : r
 }
 
 function Cc(e) {
@@ -5246,15 +5236,15 @@
 }
 
 function fb(e) {
     let t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : "px";
     if (!(e == null || e === "")) return isNaN(+e) ? String(e) : isFinite(+e) ? `${Number(e)}${t}` : void 0
 }
 
-function Ya(e) {
+function $a(e) {
     return e !== null && typeof e == "object" && !Array.isArray(e)
 }
 
 function _b(e) {
     return e && "$el" in e ? e.$el : e
 }
 const pb = Object.freeze({
@@ -5292,15 +5282,15 @@
         backspace: "Backspace",
         insert: "Insert",
         pageup: "PageUp",
         pagedown: "PageDown",
         shift: "Shift"
     });
 
-function Co(e, t) {
+function wo(e, t) {
     return t.every(n => e.hasOwnProperty(n))
 }
 
 function kc(e, t, n) {
     const r = Object.create(null),
         o = Object.create(null);
     for (const a in e) t.some(s => s instanceof RegExp ? s.test(a) : s === a) && !(n != null && n.some(s => s === a)) ? r[a] = e[a] : o[a] = e[a];
@@ -5329,15 +5319,15 @@
 }
 
 function yb(e) {
     const t = e.toString().trim();
     return t.includes(".") ? t.length - t.indexOf(".") - 1 : 0
 }
 
-function Qa(e, t) {
+function Ya(e, t) {
     let n = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : "0";
     return e + n.repeat(Math.max(0, t - e.length))
 }
 
 function m_(e) {
     let t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : 1;
     const n = [];
@@ -5351,15 +5341,15 @@
         t = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : {},
         n = arguments.length > 2 ? arguments[2] : void 0;
     const r = {};
     for (const o in e) r[o] = e[o];
     for (const o in t) {
         const a = e[o],
             s = t[o];
-        if (Ya(a) && Ya(s)) {
+        if ($a(a) && $a(s)) {
             r[o] = et(a, s, n);
             continue
         }
         if (Array.isArray(a) && Array.isArray(s) && n) {
             r[o] = n(a, s);
             continue
         }
@@ -5376,67 +5366,67 @@
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : "";
     if (tn.cache.has(e)) return tn.cache.get(e);
     const t = e.replace(/[^a-z]/gi, "-").replace(/\B([A-Z])/g, "-$1").toLowerCase();
     return tn.cache.set(e, t), t
 }
 tn.cache = new Map;
 
-function ko(e, t) {
+function Co(e, t) {
     if (!t || typeof t != "object") return [];
-    if (Array.isArray(t)) return t.map(n => ko(e, n)).flat(1);
-    if (Array.isArray(t.children)) return t.children.map(n => ko(e, n)).flat(1);
+    if (Array.isArray(t)) return t.map(n => Co(e, n)).flat(1);
+    if (Array.isArray(t.children)) return t.children.map(n => Co(e, n)).flat(1);
     if (t.component) {
         if (Object.getOwnPropertySymbols(t.component.provides).includes(e)) return [t.component];
-        if (t.component.subTree) return ko(e, t.component.subTree).flat(1)
+        if (t.component.subTree) return Co(e, t.component.subTree).flat(1)
     }
     return []
 }
-var Tr = new WeakMap,
+var vr = new WeakMap,
     un = new WeakMap;
 class vb {
     constructor(t) {
-        $a(this, Tr, {
+        Xa(this, vr, {
             writable: !0,
             value: []
-        }), $a(this, un, {
+        }), Xa(this, un, {
             writable: !0,
             value: 0
         }), this.size = t
     }
     push(t) {
-        jt(this, Tr)[jt(this, un)] = t, a_(this, un, (jt(this, un) + 1) % this.size)
+        jt(this, vr)[jt(this, un)] = t, a_(this, un, (jt(this, un) + 1) % this.size)
     }
     values() {
-        return jt(this, Tr).slice(jt(this, un)).concat(jt(this, Tr).slice(0, jt(this, un)))
+        return jt(this, vr).slice(jt(this, un)).concat(jt(this, vr).slice(0, jt(this, un)))
     }
 }
 
 function Tb(e) {
     const t = Xe({}),
         n = re(e);
-    return to(() => {
+    return eo(() => {
         for (const r in n.value) t[r] = n.value[r]
     }, {
         flush: "sync"
-    }), ki(t)
+    }), Ci(t)
 }
 
 function Sb(e, t) {
     return e.includes(t)
 }
 const f_ = /^on[^a-z]/,
     Ab = e => f_.test(e);
 
 function Pb(e) {
     return e[2].toLowerCase() + e.slice(3)
 }
 const Eb = () => [Function, Array];
 
 function Mb(e, t) {
-    return t = "on" + ur(t), !!(e[t] || e[`${t}Once`] || e[`${t}Capture`] || e[`${t}OnceCapture`] || e[`${t}CaptureOnce`])
+    return t = "on" + cr(t), !!(e[t] || e[`${t}Once`] || e[`${t}Capture`] || e[`${t}OnceCapture`] || e[`${t}CaptureOnce`])
 }
 
 function wb(e) {
     for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
     if (Array.isArray(e))
         for (const o of e) o(...n);
     else typeof e == "function" && e(...n)
@@ -5461,17 +5451,17 @@
         u ? u.focus() : p_(e, t === "next" ? "first" : "last")
     }
 }
 
 function Cb(e, t) {
     t = Array.isArray(t) ? t.slice(0, -1).map(n => `'${n}'`).join(", ") + ` or '${t.at(-1)}'` : `'${t}'`
 }
-const Vr = .20689655172413793,
-    h_ = e => e > Vr ** 3 ? Math.cbrt(e) : e / (3 * Vr ** 2) + 4 / 29,
-    z_ = e => e > Vr ? e ** 3 : 3 * Vr ** 2 * (e - 4 / 29);
+const Fr = .20689655172413793,
+    h_ = e => e > Fr ** 3 ? Math.cbrt(e) : e / (3 * Fr ** 2) + 4 / 29,
+    z_ = e => e > Fr ? e ** 3 : 3 * Fr ** 2 * (e - 4 / 29);
 
 function Dc(e) {
     const t = h_,
         n = t(e[1]);
     return [116 * n - 16, 500 * (t(e[0] / .95047) - n), 200 * (n - t(e[2] / 1.08883))]
 }
 
@@ -5501,15 +5491,15 @@
     return {
         r: t[0],
         g: t[1],
         b: t[2]
     }
 }
 
-function Xi(e) {
+function Ki(e) {
     let {
         r: t,
         g: n,
         b: r
     } = e;
     const o = [0, 0, 0],
         a = v_,
@@ -5518,81 +5508,81 @@
     for (let u = 0; u < 3; ++u) o[u] = s[u][0] * t + s[u][1] * n + s[u][2] * r;
     return o
 }
 
 function kb(e) {
     return !!e && /^(#|var\(--|(rgb|hsl)a?\()/.test(e)
 }
-const Za = /^(?<fn>(?:rgb|hsl)a?)\((?<values>.+)\)/,
+const Qa = /^(?<fn>(?:rgb|hsl)a?)\((?<values>.+)\)/,
     T_ = {
         rgb: (e, t, n, r) => ({
             r: e,
             g: t,
             b: n,
             a: r
         }),
         rgba: (e, t, n, r) => ({
             r: e,
             g: t,
             b: n,
             a: r
         }),
-        hsl: (e, t, n, r) => Ja({
+        hsl: (e, t, n, r) => Za({
             h: e,
             s: t,
             l: n,
             a: r
         }),
-        hsla: (e, t, n, r) => Ja({
+        hsla: (e, t, n, r) => Za({
             h: e,
             s: t,
             l: n,
             a: r
         }),
-        hsv: (e, t, n, r) => or({
+        hsv: (e, t, n, r) => rr({
             h: e,
             s: t,
             v: n,
             a: r
         }),
-        hsva: (e, t, n, r) => or({
+        hsva: (e, t, n, r) => rr({
             h: e,
             s: t,
             v: n,
             a: r
         })
     };
 
 function Qt(e) {
     if (typeof e == "number") return {
         r: (e & 16711680) >> 16,
         g: (e & 65280) >> 8,
         b: e & 255
     };
-    if (typeof e == "string" && Za.test(e)) {
+    if (typeof e == "string" && Qa.test(e)) {
         const {
             groups: t
-        } = e.match(Za), {
+        } = e.match(Qa), {
             fn: n,
             values: r
         } = t, o = r.split(/,\s*/).map(a => a.endsWith("%") && ["hsl", "hsla", "hsv", "hsva"].includes(n) ? parseFloat(a) / 100 : parseFloat(a));
         return T_[n](...o)
     } else if (typeof e == "string") {
         let t = e.startsWith("#") ? e.slice(1) : e;
         return [3, 4].includes(t.length) ? t = t.split("").map(n => n + n).join("") : [6, 8].includes(t.length), A_(t)
     } else if (typeof e == "object") {
-        if (Co(e, ["r", "g", "b"])) return e;
-        if (Co(e, ["h", "s", "l"])) return or(Gc(e));
-        if (Co(e, ["h", "s", "v"])) return or(e)
+        if (wo(e, ["r", "g", "b"])) return e;
+        if (wo(e, ["h", "s", "l"])) return rr(Gc(e));
+        if (wo(e, ["h", "s", "v"])) return rr(e)
     }
     throw new TypeError(`Invalid color: ${e==null?e:String(e)||e.constructor.name}
 Expected #hex, #hexa, rgb(), rgba(), hsl(), hsla(), object or number`)
 }
 
-function or(e) {
+function rr(e) {
     const {
         h: t,
         s: n,
         v: r,
         a: o
     } = e, a = u => {
         const c = (u + t / 60) % 6;
@@ -5602,16 +5592,16 @@
         r: s[0],
         g: s[1],
         b: s[2],
         a: o
     }
 }
 
-function Ja(e) {
-    return or(Gc(e))
+function Za(e) {
+    return rr(Gc(e))
 }
 
 function Gc(e) {
     const {
         h: t,
         s: n,
         l: r,
@@ -5621,145 +5611,145 @@
         h: t,
         s,
         v: a,
         a: o
     }
 }
 
-function Sr(e) {
+function Tr(e) {
     const t = Math.round(e).toString(16);
     return ("00".substr(0, 2 - t.length) + t).toUpperCase()
 }
 
 function S_(e) {
     let {
         r: t,
         g: n,
         b: r,
         a: o
     } = e;
-    return `#${[Sr(t),Sr(n),Sr(r),o!==void 0?Sr(Math.round(o*255)):""].join("")}`
+    return `#${[Tr(t),Tr(n),Tr(r),o!==void 0?Tr(Math.round(o*255)):""].join("")}`
 }
 
 function A_(e) {
     e = P_(e);
     let [t, n, r, o] = m_(e, 2).map(a => parseInt(a, 16));
     return o = o === void 0 ? o : o / 255, {
         r: t,
         g: n,
         b: r,
         a: o
     }
 }
 
 function P_(e) {
-    return e.startsWith("#") && (e = e.slice(1)), e = e.replace(/([^0-9a-f])/gi, "F"), (e.length === 3 || e.length === 4) && (e = e.split("").map(t => t + t).join("")), e.length !== 6 && (e = Qa(Qa(e, 6), 8, "F")), e
+    return e.startsWith("#") && (e = e.slice(1)), e = e.replace(/([^0-9a-f])/gi, "F"), (e.length === 3 || e.length === 4) && (e = e.split("").map(t => t + t).join("")), e.length !== 6 && (e = Ya(Ya(e, 6), 8, "F")), e
 }
 
 function E_(e, t) {
-    const n = Dc(Xi(e));
+    const n = Dc(Ki(e));
     return n[0] = n[0] + t * 10, Oc(Ic(n))
 }
 
 function M_(e, t) {
-    const n = Dc(Xi(e));
+    const n = Dc(Ki(e));
     return n[0] = n[0] - t * 10, Oc(Ic(n))
 }
 
 function w_(e) {
     const t = Qt(e);
-    return Xi(t)[1]
+    return Ki(t)[1]
 }
 
-function $i(e, t) {
+function Xi(e, t) {
     return n => Object.keys(e).reduce((r, o) => {
         const s = typeof e[o] == "object" && e[o] != null && !Array.isArray(e[o]) ? e[o] : {
             type: e[o]
         };
         return n && o in n ? r[o] = {
             ...s,
             default: n[o]
         } : r[o] = s, t && !r[o].source && (r[o].source = t), r
     }, {})
 }
 
-function dr(e) {
+function mr(e) {
     if (e._setup = e._setup ?? e.setup, !e.name) return e;
     if (e._setup) {
-        e.props = $i(e.props ?? {}, e.name)();
+        e.props = Xi(e.props ?? {}, e.name)();
         const t = Object.keys(e.props);
         e.filterProps = function(r) {
             return kc(r, t, ["class", "style"])
         }, e.props._as = String, e.setup = function(r, o) {
-            const a = Yi();
+            const a = $i();
             if (!a.value) return e._setup(r, o);
             const {
                 props: s,
                 provideSubDefaults: u
             } = R_(r, r._as ?? e.name, a), c = e._setup(s, o);
             return u(), c
         }
     }
     return e
 }
 
 function C_() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : !0;
-    return t => (e ? dr : no)(t)
+    return t => (e ? mr : to)(t)
 }
 
 function on(e, t) {
-    const n = On();
+    const n = In();
     if (!n) throw new Error(`[Vuetify] ${e} ${t||"must be called from inside a setup function"}`);
     return n
 }
 
 function Db() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : "composables";
     const t = on(e).type;
     return tn((t == null ? void 0 : t.aliasName) || (t == null ? void 0 : t.name))
 }
 let Rc = 0,
-    Or = new WeakMap;
+    Ir = new WeakMap;
 
 function Lc() {
     const e = on("getUid");
-    if (Or.has(e)) return Or.get(e); {
+    if (Ir.has(e)) return Ir.get(e); {
         const t = Rc++;
-        return Or.set(e, t), t
+        return Ir.set(e, t), t
     }
 }
 Lc.reset = () => {
-    Rc = 0, Or = new WeakMap
+    Rc = 0, Ir = new WeakMap
 };
 const yt = typeof window < "u",
     Ib = yt && "IntersectionObserver" in window,
     k_ = yt && ("ontouchstart" in window || window.navigator.maxTouchPoints > 0),
     Ob = yt && typeof CSS < "u" && typeof CSS.supports < "u" && CSS.supports("selector(:focus-visible)");
 
 function D_(e) {
     const {
         provides: t
     } = on("injectSelf");
     if (t && e in t) return t[e]
 }
-const ir = Symbol.for("vuetify:defaults");
+const or = Symbol.for("vuetify:defaults");
 
 function I_(e) {
     return Me(e)
 }
 
-function Yi() {
-    const e = ke(ir);
+function $i() {
+    const e = ke(or);
     if (!e) throw new Error("[Vuetify] Could not find defaults instance");
     return e
 }
 
 function O_(e, t) {
-    const n = Yi(),
+    const n = $i(),
         r = Me(e),
         o = re(() => {
             if (lt(t == null ? void 0 : t.disabled)) return n.value;
             const s = lt(t == null ? void 0 : t.scoped),
                 u = lt(t == null ? void 0 : t.reset),
                 c = lt(t == null ? void 0 : t.root);
             let l = et(r.value, {
@@ -5771,88 +5761,88 @@
                 for (let m = 0; m <= d && !(!l || !("prev" in l)); m++) l = l.prev;
                 return l && typeof c == "string" && c in l && (l = et(et(l, {
                     prev: l
                 }), l[c])), l
             }
             return l.prev ? et(l.prev, l) : l
         });
-    return Pn(ir, o), o
+    return An(or, o), o
 }
 
 function G_(e, t) {
     var n, r;
     return typeof((n = e.props) == null ? void 0 : n[t]) < "u" || typeof((r = e.props) == null ? void 0 : r[tn(t)]) < "u"
 }
 
 function R_() {
     let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : {},
         t = arguments.length > 1 ? arguments[1] : void 0,
-        n = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : Yi();
+        n = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : $i();
     const r = on("useDefaults");
     if (t = t ?? r.type.name ?? r.type.__name, !t) throw new Error("[Vuetify] Could not determine component name");
     const o = re(() => {
             var c;
             return (c = n.value) == null ? void 0 : c[e._as ?? t]
         }),
         a = new Proxy(e, {
             get(c, l) {
                 var m, f, _, p;
                 const d = Reflect.get(c, l);
                 return l === "class" || l === "style" ? [(m = o.value) == null ? void 0 : m[l], d].filter(b => b != null) : typeof l == "string" && !G_(r.vnode, l) ? ((f = o.value) == null ? void 0 : f[l]) ?? ((p = (_ = n.value) == null ? void 0 : _.global) == null ? void 0 : p[l]) ?? d : d
             }
         }),
         s = Jt();
-    to(() => {
+    eo(() => {
         if (o.value) {
             const c = Object.entries(o.value).filter(l => {
                 let [d] = l;
                 return d.startsWith(d[0].toUpperCase())
             });
             c.length && (s.value = Object.fromEntries(c))
         }
     });
 
     function u() {
         Ec(s, () => {
             var c;
-            O_(et(((c = D_(ir)) == null ? void 0 : c.value) ?? {}, s.value))
+            O_(et(((c = D_(or)) == null ? void 0 : c.value) ?? {}, s.value))
         })
     }
     return {
         props: a,
         provideSubDefaults: u
     }
 }
 const Gb = ["sm", "md", "lg", "xl", "xxl"],
-    Zo = Symbol.for("vuetify:display"),
-    es = {
+    Qo = Symbol.for("vuetify:display"),
+    Ja = {
         mobileBreakpoint: "lg",
         thresholds: {
             xs: 0,
             sm: 600,
             md: 960,
             lg: 1280,
             xl: 1920,
             xxl: 2560
         }
     },
     L_ = function() {
-        let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : es;
-        return et(es, e)
+        let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : Ja;
+        return et(Ja, e)
     };
 
-function ts(e) {
+function es(e) {
     return yt && !e ? window.innerWidth : typeof e == "object" && e.clientWidth || 0
 }
 
-function ns(e) {
+function ts(e) {
     return yt && !e ? window.innerHeight : typeof e == "object" && e.clientHeight || 0
 }
 
-function rs(e) {
+function ns(e) {
     const t = yt && !e ? window.navigator.userAgent : "ssr";
 
     function n(p) {
         return !!t.match(p)
     }
     const r = n(/android/i),
         o = n(/iphone|ipad|ipod/i),
@@ -5882,45 +5872,45 @@
     }
 }
 
 function B_(e, t) {
     const {
         thresholds: n,
         mobileBreakpoint: r
-    } = L_(e), o = Jt(ns(t)), a = Jt(rs(t)), s = Xe({}), u = Jt(ts(t));
+    } = L_(e), o = Jt(ts(t)), a = Jt(ns(t)), s = Xe({}), u = Jt(es(t));
 
     function c() {
-        o.value = ns(), u.value = ts()
+        o.value = ts(), u.value = es()
     }
 
     function l() {
-        c(), a.value = rs()
+        c(), a.value = ns()
     }
-    return to(() => {
+    return eo(() => {
         const d = u.value < n.sm,
             m = u.value < n.md && !d,
             f = u.value < n.lg && !(m || d),
             _ = u.value < n.xl && !(f || m || d),
             p = u.value < n.xxl && !(_ || f || m || d),
             b = u.value >= n.xxl,
             T = d ? "xs" : m ? "sm" : f ? "md" : _ ? "lg" : p ? "xl" : "xxl",
             v = typeof r == "number" ? r : n[r],
             A = u.value < v;
         s.xs = d, s.sm = m, s.md = f, s.lg = _, s.xl = p, s.xxl = b, s.smAndUp = !d, s.mdAndUp = !(d || m), s.lgAndUp = !(d || m || f), s.xlAndUp = !(d || m || f || _), s.smAndDown = !(f || _ || p || b), s.mdAndDown = !(_ || p || b), s.lgAndDown = !(p || b), s.xlAndDown = !b, s.name = T, s.height = o.value, s.width = u.value, s.mobile = A, s.mobileBreakpoint = r, s.platform = a.value, s.thresholds = n
     }), yt && window.addEventListener("resize", c, {
         passive: !0
     }), {
-        ...ki(s),
+        ...Ci(s),
         update: l,
         ssr: !!t
     }
 }
 
 function Rb() {
-    const e = ke(Zo);
+    const e = ke(Qo);
     if (!e) throw new Error("Could not find Vuetify display injection");
     return e
 }
 const Bc = {
         collapse: "mdi-chevron-up",
         complete: "mdi-check",
         cancel: "mdi-close-circle",
@@ -5961,27 +5951,27 @@
     Nc = {
         component: e => rn(xc, {
             ...e,
             class: "mdi"
         })
     },
     N_ = [String, Function, Object, Array],
-    Jo = Symbol.for("vuetify:icons"),
-    po = $i({
+    Zo = Symbol.for("vuetify:icons"),
+    _o = Xi({
         icon: {
             type: N_
         },
         tag: {
             type: String,
             required: !0
         }
     }, "icon"),
-    os = C_()({
+    rs = C_()({
         name: "VComponentIcon",
-        props: po(),
+        props: _o(),
         setup(e, t) {
             let {
                 slots: n
             } = t;
             return () => {
                 const r = e.icon;
                 return fe(e.tag, null, {
@@ -5989,23 +5979,23 @@
                         var o;
                         return [e.icon ? fe(r, null, null) : (o = n.default) == null ? void 0 : o.call(n)]
                     }
                 })
             }
         }
     }),
-    Hc = dr({
+    Hc = mr({
         name: "VSvgIcon",
         inheritAttrs: !1,
-        props: po(),
+        props: _o(),
         setup(e, t) {
             let {
                 attrs: n
             } = t;
-            return () => fe(e.tag, uc(n, {
+            return () => fe(e.tag, cc(n, {
                 style: null
             }), {
                 default: () => [fe("svg", {
                     class: "v-icon__svg",
                     xmlns: "http://www.w3.org/2000/svg",
                     viewBox: "0 0 24 24",
                     role: "img",
@@ -6017,26 +6007,26 @@
                     d: r
                 }, null)) : fe("path", {
                     d: e.icon
                 }, null)])]
             })
         }
     }),
-    H_ = dr({
+    H_ = mr({
         name: "VLigatureIcon",
-        props: po(),
+        props: _o(),
         setup(e) {
             return () => fe(e.tag, null, {
                 default: () => [e.icon]
             })
         }
     }),
-    xc = dr({
+    xc = mr({
         name: "VClassIcon",
-        props: po(),
+        props: _o(),
         setup(e) {
             return () => fe(e.tag, {
                 class: e.icon
             }, null)
         }
     }),
     x_ = {
@@ -6059,31 +6049,31 @@
             ...Bc,
             vuetify: ["M8.2241 14.2009L12 21L22 3H14.4459L8.2241 14.2009Z", ["M7.26303 12.4733L7.00113 12L2 3H12.5261C12.5261 3 12.5261 3 12.5261 3L7.26303 12.4733Z", .6]],
             "vuetify-outline": "svg:M7.26 12.47 12.53 3H2L7.26 12.47ZM14.45 3 8.22 14.2 12 21 22 3H14.45ZM18.6 5 12 16.88 10.51 14.2 15.62 5ZM7.26 8.35 5.4 5H9.13L7.26 8.35Z"
         }
     }, e)
 }
 const Lb = e => {
-        const t = ke(Jo);
+        const t = ke(Zo);
         if (!t) throw new Error("Missing Vuetify Icons provide!");
         return {
             iconData: re(() => {
                 var c;
                 const r = lt(e);
                 if (!r) return {
-                    component: os
+                    component: rs
                 };
                 let o = r;
                 if (typeof o == "string" && (o = o.trim(), o.startsWith("$") && (o = (c = t.aliases) == null ? void 0 : c[o.slice(1)])), !o) throw new Error(`Could not find aliased icon "${r}"`);
                 if (Array.isArray(o)) return {
                     component: Hc,
                     icon: o
                 };
                 if (typeof o != "string") return {
-                    component: os,
+                    component: rs,
                     icon: o
                 };
                 const a = Object.keys(t.sets).find(l => typeof o == "string" && o.startsWith(`${l}:`)),
                     s = a ? o.slice(a.length + 1) : o;
                 return {
                     component: t.sets[a ?? t.defaultSet].component,
                     icon: s
@@ -6254,42 +6244,42 @@
             _ === f || r(_) === m || (s.value = f, a == null || a.emit(`update:${t}`, f))
         }
     });
     return Object.defineProperty(d, "externalValue", {
         get: () => l.value ? e[t] : s.value
     }), d
 }
-const is = "$vuetify.",
-    as = (e, t) => e.replace(/\{(\d+)\}/g, (n, r) => String(t[+r])),
+const os = "$vuetify.",
+    is = (e, t) => e.replace(/\{(\d+)\}/g, (n, r) => String(t[+r])),
     Fc = (e, t, n) => function(r) {
         for (var o = arguments.length, a = new Array(o > 1 ? o - 1 : 0), s = 1; s < o; s++) a[s - 1] = arguments[s];
-        if (!r.startsWith(is)) return as(r, a);
-        const u = r.replace(is, ""),
+        if (!r.startsWith(os)) return is(r, a);
+        const u = r.replace(os, ""),
             c = e.value && n.value[e.value],
             l = t.value && n.value[t.value];
-        let d = Qo(c, u, null);
-        return d || (`${r}${e.value}`, d = Qo(l, u, null)), d || (d = r), typeof d != "string" && (d = r), as(d, a)
+        let d = Yo(c, u, null);
+        return d || (`${r}${e.value}`, d = Yo(l, u, null)), d || (d = r), typeof d != "string" && (d = r), is(d, a)
     };
 
 function Vc(e, t) {
     return (n, r) => new Intl.NumberFormat([e.value, t.value], r).format(n)
 }
 
-function Do(e, t, n) {
+function ko(e, t, n) {
     const r = W_(e, t, e[t] ?? n.value);
     return r.value = e[t] ?? n.value, xe(n, o => {
         e[t] == null && (r.value = n.value)
     }), r
 }
 
 function Uc(e) {
     return t => {
-        const n = Do(t, "locale", e.current),
-            r = Do(t, "fallback", e.fallback),
-            o = Do(t, "messages", e.messages);
+        const n = ko(t, "locale", e.current),
+            r = ko(t, "fallback", e.fallback),
+            o = ko(t, "messages", e.messages);
         return {
             name: "vuetify",
             current: n,
             fallback: r,
             messages: o,
             t: Fc(n, r, o),
             n: Vc(n, r),
@@ -6319,15 +6309,15 @@
         provide: Uc({
             current: t,
             fallback: n,
             messages: r
         })
     }
 }
-const Ur = Symbol.for("vuetify:locale");
+const Vr = Symbol.for("vuetify:locale");
 
 function q_(e) {
     return e.name != null
 }
 
 function K_(e) {
     const t = e != null && e.adapter && q_(e == null ? void 0 : e.adapter) ? e == null ? void 0 : e.adapter : j_(e),
@@ -6335,15 +6325,15 @@
     return {
         ...t,
         ...n
     }
 }
 
 function Bb() {
-    const e = ke(Ur);
+    const e = ke(Vr);
     if (!e) throw new Error("[Vuetify] Could not find injected locale instance");
     return e
 }
 
 function X_(e, t) {
     const n = Me((t == null ? void 0 : t.rtl) ?? U_),
         r = re(() => n.value[e.current.value] ?? !1);
@@ -6351,64 +6341,64 @@
         isRtl: r,
         rtl: n,
         rtlClasses: re(() => `v-locale--is-${r.value?"rtl":"ltr"}`)
     }
 }
 
 function Nb() {
-    const e = ke(Ur);
+    const e = ke(Vr);
     if (!e) throw new Error("[Vuetify] Could not find injected rtl instance");
     return {
         isRtl: e.isRtl,
         rtlClasses: e.rtlClasses
     }
 }
 const mn = 2.4,
-    ss = .2126729,
-    ls = .7151522,
-    cs = .072175,
+    as = .2126729,
+    ss = .7151522,
+    ls = .072175,
     $_ = .55,
     Y_ = .58,
     Q_ = .57,
     Z_ = .62,
-    Ar = .03,
-    us = 1.45,
+    Sr = .03,
+    cs = 1.45,
     J_ = 5e-4,
     e0 = 1.25,
     t0 = 1.25,
-    ms = .078,
-    ds = 12.82051282051282,
-    Pr = .06,
-    fs = .001;
+    us = .078,
+    ms = 12.82051282051282,
+    Ar = .06,
+    ds = .001;
 
-function _s(e, t) {
+function fs(e, t) {
     const n = (e.r / 255) ** mn,
         r = (e.g / 255) ** mn,
         o = (e.b / 255) ** mn,
         a = (t.r / 255) ** mn,
         s = (t.g / 255) ** mn,
         u = (t.b / 255) ** mn;
-    let c = n * ss + r * ls + o * cs,
-        l = a * ss + s * ls + u * cs;
-    if (c <= Ar && (c += (Ar - c) ** us), l <= Ar && (l += (Ar - l) ** us), Math.abs(l - c) < J_) return 0;
+    let c = n * as + r * ss + o * ls,
+        l = a * as + s * ss + u * ls;
+    if (c <= Sr && (c += (Sr - c) ** cs), l <= Sr && (l += (Sr - l) ** cs), Math.abs(l - c) < J_) return 0;
     let d;
     if (l > c) {
         const m = (l ** $_ - c ** Y_) * e0;
-        d = m < fs ? 0 : m < ms ? m - m * ds * Pr : m - Pr
+        d = m < ds ? 0 : m < us ? m - m * ms * Ar : m - Ar
     } else {
         const m = (l ** Z_ - c ** Q_) * t0;
-        d = m > -fs ? 0 : m > -ms ? m - m * ds * Pr : m + Pr
+        d = m > -ds ? 0 : m > -us ? m - m * ms * Ar : m + Ar
     }
     return d * 100
 }
-const ar = Symbol.for("vuetify:theme"),
-    Hb = $i({
+const ir = Symbol.for("vuetify:theme"),
+    Hb = Xi({
         theme: String
     }, "theme"),
-    Bn = {
+    Ln = {
         defaultTheme: "light",
         variations: {
             colors: [],
             lighten: 0,
             darken: 0
         },
         themes: {
@@ -6483,25 +6473,25 @@
                 }
             }
         }
     };
 
 function n0() {
     var n, r;
-    let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : Bn;
+    let e = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : Ln;
     if (!e) return {
-        ...Bn,
+        ...Ln,
         isDisabled: !0
     };
     const t = {};
     for (const [o, a] of Object.entries(e.themes ?? {})) {
-        const s = a.dark || o === "dark" ? (n = Bn.themes) == null ? void 0 : n.dark : (r = Bn.themes) == null ? void 0 : r.light;
+        const s = a.dark || o === "dark" ? (n = Ln.themes) == null ? void 0 : n.dark : (r = Ln.themes) == null ? void 0 : r.light;
         t[o] = et(s, a)
     }
-    return et(Bn, {
+    return et(Ln, {
         ...e,
         themes: t
     })
 }
 
 function r0(e) {
     const t = n0(e),
@@ -6525,26 +6515,26 @@
                                 for (const A of Cc(t.variations[T], 1)) _.colors[`${p}-${T}-${A}`] = S_(v(Qt(b), A))
                             }
                     }
                 for (const p of Object.keys(_.colors)) {
                     if (/^on-[a-z]/.test(p) || _.colors[`on-${p}`]) continue;
                     const b = `on-${p}`,
                         T = Qt(_.colors[p]),
-                        v = Math.abs(_s(Qt(0), T)),
-                        A = Math.abs(_s(Qt(16777215), T));
+                        v = Math.abs(fs(Qt(0), T)),
+                        A = Math.abs(fs(Qt(16777215), T));
                     _.colors[b] = A > Math.min(v, 50) ? "#fff" : "#000"
                 }
             }
             return d
         }),
         a = re(() => o.value[n.value]),
         s = re(() => {
             const d = [];
-            a.value.dark && qt(d, ":root", ["color-scheme: dark"]), qt(d, ":root", ps(a.value));
-            for (const [p, b] of Object.entries(o.value)) qt(d, `.v-theme--${p}`, [`color-scheme: ${b.dark?"dark":"normal"}`, ...ps(b)]);
+            a.value.dark && qt(d, ":root", ["color-scheme: dark"]), qt(d, ":root", _s(a.value));
+            for (const [p, b] of Object.entries(o.value)) qt(d, `.v-theme--${p}`, [`color-scheme: ${b.dark?"dark":"normal"}`, ..._s(b)]);
             const m = [],
                 f = [],
                 _ = new Set(Object.values(o.value).flatMap(p => Object.keys(p.colors)));
             for (const p of _) /^on-[a-z]/.test(p) ? qt(f, `.${p}`, [`color: rgb(var(--v-theme-${p})) !important`]) : (qt(m, `.bg-${p}`, [`--v-theme-overlay-multiplier: var(--v-theme-${p}-overlay-multiplier)`, `background-color: rgb(var(--v-theme-${p})) !important`, `color: rgb(var(--v-theme-on-${p})) !important`]), qt(f, `.text-${p}`, [`color: rgb(var(--v-theme-${p})) !important`]), qt(f, `.border-${p}`, [`--v-border-color: var(--v-theme-${p})`]));
             return d.push(...m, ...f), d.map((p, b) => b === 0 ? p : `    ${p}`).join("")
         });
 
@@ -6563,15 +6553,15 @@
         const m = d._context.provides.usehead;
         if (m)
             if (m.push) {
                 const f = m.push(u);
                 xe(s, () => {
                     f.patch(u)
                 })
-            } else yt ? (m.addHeadObjs(re(u)), to(() => m.updateDOM())) : m.addHeadObjs(u());
+            } else yt ? (m.addHeadObjs(re(u)), eo(() => m.updateDOM())) : m.addHeadObjs(u());
         else {
             let _ = function() {
                     if (typeof document < "u" && !f) {
                         const p = document.createElement("style");
                         p.type = "text/css", p.id = "vuetify-theme-stylesheet", t.cspNonce && p.setAttribute("nonce", t.cspNonce), f = p, document.head.appendChild(f)
                     }
                     f && (f.innerHTML = s.value)
@@ -6597,56 +6587,56 @@
             current: a
         }
     }
 }
 
 function xb(e) {
     on("provideTheme");
-    const t = ke(ar, null);
+    const t = ke(ir, null);
     if (!t) throw new Error("Could not find Vuetify theme injection");
     const n = re(() => e.theme ?? (t == null ? void 0 : t.name.value)),
         r = re(() => t.isDisabled ? void 0 : `v-theme--${n.value}`),
         o = {
             ...t,
             name: n,
             themeClasses: r
         };
-    return Pn(ar, o), o
+    return An(ir, o), o
 }
 
 function o0() {
     on("useTheme");
-    const e = ke(ar, null);
+    const e = ke(ir, null);
     if (!e) throw new Error("Could not find Vuetify theme injection");
     return e
 }
 
 function qt(e, t, n) {
     e.push(`${t} {
 `, ...n.map(r => `  ${r};
 `), `}
 `)
 }
 
-function ps(e) {
+function _s(e) {
     const t = e.dark ? 2 : 1,
         n = e.dark ? 1 : 2,
         r = [];
     for (const [o, a] of Object.entries(e.colors)) {
         const s = Qt(a);
         r.push(`--v-theme-${o}: ${s.r},${s.g},${s.b}`), o.startsWith("on-") || r.push(`--v-theme-${o}-overlay-multiplier: ${w_(a)>.18?t:n}`)
     }
     for (const [o, a] of Object.entries(e.variables)) {
         const s = typeof a == "string" && a.startsWith("#") ? Qt(a) : void 0,
             u = s ? `${s.r}, ${s.g}, ${s.b}` : void 0;
         r.push(`--v-${o}: ${u??a}`)
     }
     return r
 }
-const ei = {
+const Jo = {
     "001": 1,
     AD: 1,
     AE: 6,
     AF: 6,
     AG: 0,
     AI: 1,
     AL: 1,
@@ -6797,16 +6787,16 @@
 };
 
 function i0(e, t) {
     const n = [];
     let r = [];
     const o = Wc(e),
         a = jc(e),
-        s = o.getDay() - ei[t.slice(-2).toUpperCase()],
-        u = a.getDay() - ei[t.slice(-2).toUpperCase()];
+        s = o.getDay() - Jo[t.slice(-2).toUpperCase()],
+        u = a.getDay() - Jo[t.slice(-2).toUpperCase()];
     for (let c = 0; c < s; c++) {
         const l = new Date(o);
         l.setDate(l.getDate() - (s - c)), r.push(l)
     }
     for (let c = 1; c <= a.getDate(); c++) {
         const l = new Date(e.getFullYear(), e.getMonth(), c);
         r.push(l), r.length === 7 && (n.push(r), r = [])
@@ -6840,21 +6830,21 @@
     if (e instanceof Date) return e;
     if (typeof e == "string") {
         let t;
         if (s0.test(e) ? t = Date.parse(a0(e)) : t = Date.parse(e), !isNaN(t)) return new Date(t)
     }
     return null
 }
-const hs = new Date(2e3, 0, 2);
+const ps = new Date(2e3, 0, 2);
 
 function c0(e) {
-    const t = ei[e.slice(-2).toUpperCase()];
+    const t = Jo[e.slice(-2).toUpperCase()];
     return Cc(7).map(n => {
-        const r = new Date(hs);
-        return r.setDate(hs.getDate() + t + n), new Intl.DateTimeFormat(e, {
+        const r = new Date(ps);
+        return r.setDate(ps.getDate() + t + n), new Intl.DateTimeFormat(e, {
             weekday: "short"
         }).format(r)
     })
 }
 
 function u0(e, t, n) {
     const r = new Date(e);
@@ -6927,31 +6917,31 @@
 }
 
 function h0(e) {
     return new Date(e.getFullYear(), 11, 31)
 }
 
 function z0(e, t) {
-    return ti(e, t[0]) && g0(e, t[1])
+    return ei(e, t[0]) && g0(e, t[1])
 }
 
 function b0(e) {
     const t = new Date(e);
     return t instanceof Date && !isNaN(t.getTime())
 }
 
-function ti(e, t) {
+function ei(e, t) {
     return e.getTime() > t.getTime()
 }
 
 function g0(e, t) {
     return e.getTime() < t.getTime()
 }
 
-function zs(e, t) {
+function hs(e, t) {
     return e.getTime() === t.getTime()
 }
 
 function y0(e, t) {
     return e.getDate() === t.getDate() && e.getMonth() === t.getMonth() && e.getFullYear() === t.getFullYear()
 }
 
@@ -6994,27 +6984,27 @@
     endOfMonth(t) {
         return jc(t)
     }
     format(t, n) {
         return u0(t, n, this.locale)
     }
     isEqual(t, n) {
-        return zs(t, n)
+        return hs(t, n)
     }
     isValid(t) {
         return b0(t)
     }
     isWithinRange(t, n) {
         return z0(t, n)
     }
     isAfter(t, n) {
-        return ti(t, n)
+        return ei(t, n)
     }
     isBefore(t, n) {
-        return !ti(t, n) && !zs(t, n)
+        return !ei(t, n) && !hs(t, n)
     }
     isSameDay(t, n) {
         return y0(t, n)
     }
     isSameMonth(t, n) {
         return v0(t, n)
     }
@@ -7036,15 +7026,15 @@
     startOfYear(t) {
         return p0(t)
     }
     endOfYear(t) {
         return h0(t)
     }
 }
-const bs = Symbol.for("vuetify:date-adapter");
+const zs = Symbol.for("vuetify:date-adapter");
 
 function P0(e) {
     return et({
         adapter: A0,
         locale: {
             af: "af-ZA",
             bg: "bg-BG",
@@ -7098,41 +7088,41 @@
         components: a = {},
         directives: s = {}
     } = r, u = I_(r.defaults), c = B_(r.display, r.ssr), l = r0(r.theme), d = F_(r.icons), m = K_(r.locale), f = P0(r.date);
     return {
         install: p => {
             for (const b in s) p.directive(b, s[b]);
             for (const b in a) p.component(b, a[b]);
-            for (const b in o) p.component(b, dr({
+            for (const b in o) p.component(b, mr({
                 ...o[b],
                 name: b,
                 aliasName: o[b].name
             }));
-            if (l.install(p), p.provide(ir, u), p.provide(Zo, c), p.provide(ar, l), p.provide(Jo, d), p.provide(Ur, m), p.provide(bs, f), yt && r.ssr)
+            if (l.install(p), p.provide(or, u), p.provide(Qo, c), p.provide(ir, l), p.provide(Zo, d), p.provide(Vr, m), p.provide(zs, f), yt && r.ssr)
                 if (p.$nuxt) p.$nuxt.hook("app:suspense:resolve", () => {
                     c.update()
                 });
                 else {
                     const {
                         mount: b
                     } = p;
                     p.mount = function() {
                         const T = b(...arguments);
-                        return Ii(() => c.update()), p.mount = b, T
+                        return Di(() => c.update()), p.mount = b, T
                     }
                 } Lc.reset(), p.mixin({
                 computed: {
                     $vuetify() {
                         return Xe({
-                            defaults: dn.call(this, ir),
-                            display: dn.call(this, Zo),
-                            theme: dn.call(this, ar),
-                            icons: dn.call(this, Jo),
-                            locale: dn.call(this, Ur),
-                            date: dn.call(this, bs)
+                            defaults: dn.call(this, or),
+                            display: dn.call(this, Qo),
+                            theme: dn.call(this, ir),
+                            icons: dn.call(this, Zo),
+                            locale: dn.call(this, Vr),
+                            date: dn.call(this, zs)
                         })
                     }
                 }
             })
         },
         defaults: u,
         display: c,
@@ -7309,32 +7299,32 @@
     },
     M0 = function(t) {
         return !t || typeof t == "string" ? !1 : t instanceof Array || Array.isArray(t) || t.length >= 0 && (t.splice instanceof Function || Object.getOwnPropertyDescriptor(t, t.length - 1) && t.constructor.name !== "String")
     },
     w0 = M0,
     C0 = Array.prototype.concat,
     k0 = Array.prototype.slice,
-    gs = $c.exports = function(t) {
+    bs = $c.exports = function(t) {
         for (var n = [], r = 0, o = t.length; r < o; r++) {
             var a = t[r];
             w0(a) ? n = C0.call(n, k0.call(a)) : n.push(a)
         }
         return n
     };
-gs.wrap = function(e) {
+bs.wrap = function(e) {
     return function() {
-        return e(gs(arguments))
+        return e(bs(arguments))
     }
 };
 var D0 = $c.exports,
-    qn = Xc,
-    fr = D0,
+    jn = Xc,
+    dr = D0,
     Yc = Object.hasOwnProperty,
     Qc = Object.create(null);
-for (var Io in qn) Yc.call(qn, Io) && (Qc[qn[Io]] = Io);
+for (var Do in jn) Yc.call(jn, Do) && (Qc[jn[Do]] = Do);
 var $e = Kc.exports = {
     to: {},
     get: {}
 };
 $e.get = function(e) {
     var t = e.substring(0, 3).toLowerCase(),
         n, r;
@@ -7374,15 +7364,15 @@
         l && (s[3] = parseInt(l + l, 16) / 255)
     } else if (u = e.match(r)) {
         for (c = 0; c < 3; c++) s[c] = parseInt(u[c + 1], 0);
         u[4] && (u[5] ? s[3] = parseFloat(u[4]) * .01 : s[3] = parseFloat(u[4]))
     } else if (u = e.match(o)) {
         for (c = 0; c < 3; c++) s[c] = Math.round(parseFloat(u[c + 1]) * 2.55);
         u[4] && (u[5] ? s[3] = parseFloat(u[4]) * .01 : s[3] = parseFloat(u[4]))
-    } else return (u = e.match(a)) ? u[1] === "transparent" ? [0, 0, 0, 0] : Yc.call(qn, u[1]) ? (s = qn[u[1]], s[3] = 1, s) : null : null;
+    } else return (u = e.match(a)) ? u[1] === "transparent" ? [0, 0, 0, 0] : Yc.call(jn, u[1]) ? (s = jn[u[1]], s[3] = 1, s) : null : null;
     for (c = 0; c < 3; c++) s[c] = Lt(s[c], 0, 255);
     return s[3] = Lt(s[3], 0, 1), s
 };
 $e.get.hsl = function(e) {
     if (!e) return null;
     var t = /^hsla?\(\s*([+-]?(?:\d{0,3}\.)?\d+)(?:deg)?\s*,?\s*([+-]?[\d\.]+)%\s*,?\s*([+-]?[\d\.]+)%\s*(?:[,|\/]\s*([+-]?(?=\.\d|\d)(?:0|[1-9]\d*)?(?:\.\d*)?(?:[eE][+-]?\d+)?)\s*)?\)$/,
         n = e.match(t);
@@ -7407,53 +7397,53 @@
             s = Lt(parseFloat(n[3]), 0, 100),
             u = Lt(isNaN(r) ? 1 : r, 0, 1);
         return [o, a, s, u]
     }
     return null
 };
 $e.to.hex = function() {
-    var e = fr(arguments);
-    return "#" + Er(e[0]) + Er(e[1]) + Er(e[2]) + (e[3] < 1 ? Er(Math.round(e[3] * 255)) : "")
+    var e = dr(arguments);
+    return "#" + Pr(e[0]) + Pr(e[1]) + Pr(e[2]) + (e[3] < 1 ? Pr(Math.round(e[3] * 255)) : "")
 };
 $e.to.rgb = function() {
-    var e = fr(arguments);
+    var e = dr(arguments);
     return e.length < 4 || e[3] === 1 ? "rgb(" + Math.round(e[0]) + ", " + Math.round(e[1]) + ", " + Math.round(e[2]) + ")" : "rgba(" + Math.round(e[0]) + ", " + Math.round(e[1]) + ", " + Math.round(e[2]) + ", " + e[3] + ")"
 };
 $e.to.rgb.percent = function() {
-    var e = fr(arguments),
+    var e = dr(arguments),
         t = Math.round(e[0] / 255 * 100),
         n = Math.round(e[1] / 255 * 100),
         r = Math.round(e[2] / 255 * 100);
     return e.length < 4 || e[3] === 1 ? "rgb(" + t + "%, " + n + "%, " + r + "%)" : "rgba(" + t + "%, " + n + "%, " + r + "%, " + e[3] + ")"
 };
 $e.to.hsl = function() {
-    var e = fr(arguments);
+    var e = dr(arguments);
     return e.length < 4 || e[3] === 1 ? "hsl(" + e[0] + ", " + e[1] + "%, " + e[2] + "%)" : "hsla(" + e[0] + ", " + e[1] + "%, " + e[2] + "%, " + e[3] + ")"
 };
 $e.to.hwb = function() {
-    var e = fr(arguments),
+    var e = dr(arguments),
         t = "";
     return e.length >= 4 && e[3] !== 1 && (t = ", " + e[3]), "hwb(" + e[0] + ", " + e[1] + "%, " + e[2] + "%" + t + ")"
 };
 $e.to.keyword = function(e) {
     return Qc[e.slice(0, 3)]
 };
 
 function Lt(e, t, n) {
     return Math.min(Math.max(t, e), n)
 }
 
-function Er(e) {
+function Pr(e) {
     var t = Math.round(e).toString(16).toUpperCase();
     return t.length < 2 ? "0" + t : t
 }
 var I0 = Kc.exports;
-const sr = Xc,
+const ar = Xc,
     Zc = {};
-for (const e of Object.keys(sr)) Zc[sr[e]] = e;
+for (const e of Object.keys(ar)) Zc[ar[e]] = e;
 const V = {
     rgb: {
         channels: 3,
         labels: "rgb"
     },
     hsl: {
         channels: 3,
@@ -7574,23 +7564,23 @@
     return (e[0] - t[0]) ** 2 + (e[1] - t[1]) ** 2 + (e[2] - t[2]) ** 2
 }
 V.rgb.keyword = function(e) {
     const t = Zc[e];
     if (t) return t;
     let n = 1 / 0,
         r;
-    for (const o of Object.keys(sr)) {
-        const a = sr[o],
+    for (const o of Object.keys(ar)) {
+        const a = ar[o],
             s = O0(e, a);
         s < n && (n = s, r = o)
     }
     return r
 };
 V.keyword.rgb = function(e) {
-    return sr[e]
+    return ar[e]
 };
 V.rgb.xyz = function(e) {
     let t = e[0] / 255,
         n = e[1] / 255,
         r = e[2] / 255;
     t = t > .04045 ? ((t + .055) / 1.055) ** 2.4 : t / 12.92, n = n > .04045 ? ((n + .055) / 1.055) ** 2.4 : n / 12.92, r = r > .04045 ? ((r + .055) / 1.055) ** 2.4 : r / 12.92;
     const o = t * .4124 + n * .3576 + r * .1805,
@@ -7916,32 +7906,32 @@
     const t = Math.round(e[0] / 100 * 255) & 255,
         r = ((t << 16) + (t << 8) + t).toString(16).toUpperCase();
     return "000000".substring(r.length) + r
 };
 V.rgb.gray = function(e) {
     return [(e[0] + e[1] + e[2]) / 3 / 255 * 100]
 };
-const Wr = Jc;
+const Ur = Jc;
 
 function G0() {
     const e = {},
-        t = Object.keys(Wr);
+        t = Object.keys(Ur);
     for (let n = t.length, r = 0; r < n; r++) e[t[r]] = {
         distance: -1,
         parent: null
     };
     return e
 }
 
 function R0(e) {
     const t = G0(),
         n = [e];
     for (t[e].distance = 0; n.length;) {
         const r = n.pop(),
-            o = Object.keys(Wr[r]);
+            o = Object.keys(Ur[r]);
         for (let a = o.length, s = 0; s < a; s++) {
             const u = o[s],
                 c = t[u];
             c.distance === -1 && (c.distance = t[r].distance + 1, c.parent = r, n.unshift(u))
         }
     }
     return t
@@ -7951,33 +7941,33 @@
     return function(n) {
         return t(e(n))
     }
 }
 
 function B0(e, t) {
     const n = [t[e].parent, e];
-    let r = Wr[t[e].parent][e],
+    let r = Ur[t[e].parent][e],
         o = t[e].parent;
-    for (; t[o].parent;) n.unshift(t[o].parent), r = L0(Wr[t[o].parent][o], r), o = t[o].parent;
+    for (; t[o].parent;) n.unshift(t[o].parent), r = L0(Ur[t[o].parent][o], r), o = t[o].parent;
     return r.conversion = n, r
 }
 var N0 = function(e) {
     const t = R0(e),
         n = {},
         r = Object.keys(t);
     for (let o = r.length, a = 0; a < o; a++) {
         const s = r[a];
         t[s].parent !== null && (n[s] = B0(s, t))
     }
     return n
 };
-const ni = Jc,
+const ti = Jc,
     H0 = N0,
-    pn = {},
-    x0 = Object.keys(ni);
+    _n = {},
+    x0 = Object.keys(ti);
 
 function F0(e) {
     const t = function(...n) {
         const r = n[0];
         return r == null ? r : (r.length > 1 && (n = r), e(n))
     };
     return "conversion" in e && (t.conversion = e.conversion), t
@@ -7992,85 +7982,85 @@
         if (typeof o == "object")
             for (let a = o.length, s = 0; s < a; s++) o[s] = Math.round(o[s]);
         return o
     };
     return "conversion" in e && (t.conversion = e.conversion), t
 }
 x0.forEach(e => {
-    pn[e] = {}, Object.defineProperty(pn[e], "channels", {
-        value: ni[e].channels
-    }), Object.defineProperty(pn[e], "labels", {
-        value: ni[e].labels
+    _n[e] = {}, Object.defineProperty(_n[e], "channels", {
+        value: ti[e].channels
+    }), Object.defineProperty(_n[e], "labels", {
+        value: ti[e].labels
     });
     const t = H0(e);
     Object.keys(t).forEach(r => {
         const o = t[r];
-        pn[e][r] = V0(o), pn[e][r].raw = F0(o)
+        _n[e][r] = V0(o), _n[e][r].raw = F0(o)
     })
 });
-var U0 = pn;
-const hn = I0,
+var U0 = _n;
+const pn = I0,
     Ke = U0,
     eu = ["keyword", "gray", "hex"],
-    ri = {};
-for (const e of Object.keys(Ke)) ri[[...Ke[e].labels].sort().join("")] = e;
-const jr = {};
+    ni = {};
+for (const e of Object.keys(Ke)) ni[[...Ke[e].labels].sort().join("")] = e;
+const Wr = {};
 
 function Ee(e, t) {
     if (!(this instanceof Ee)) return new Ee(e, t);
     if (t && t in eu && (t = null), t && !(t in Ke)) throw new Error("Unknown model: " + t);
     let n, r;
     if (e == null) this.model = "rgb", this.color = [0, 0, 0], this.valpha = 1;
     else if (e instanceof Ee) this.model = e.model, this.color = [...e.color], this.valpha = e.valpha;
     else if (typeof e == "string") {
-        const o = hn.get(e);
+        const o = pn.get(e);
         if (o === null) throw new Error("Unable to parse color from string: " + e);
         this.model = o.model, r = Ke[this.model].channels, this.color = o.value.slice(0, r), this.valpha = typeof o.value[r] == "number" ? o.value[r] : 1
     } else if (e.length > 0) {
         this.model = t || "rgb", r = Ke[this.model].channels;
         const o = Array.prototype.slice.call(e, 0, r);
-        this.color = oi(o, r), this.valpha = typeof e[r] == "number" ? e[r] : 1
+        this.color = ri(o, r), this.valpha = typeof e[r] == "number" ? e[r] : 1
     } else if (typeof e == "number") this.model = "rgb", this.color = [e >> 16 & 255, e >> 8 & 255, e & 255], this.valpha = 1;
     else {
         this.valpha = 1;
         const o = Object.keys(e);
         "alpha" in e && (o.splice(o.indexOf("alpha"), 1), this.valpha = typeof e.alpha == "number" ? e.alpha : 0);
         const a = o.sort().join("");
-        if (!(a in ri)) throw new Error("Unable to parse color from object: " + JSON.stringify(e));
-        this.model = ri[a];
+        if (!(a in ni)) throw new Error("Unable to parse color from object: " + JSON.stringify(e));
+        this.model = ni[a];
         const {
             labels: s
         } = Ke[this.model], u = [];
         for (n = 0; n < s.length; n++) u.push(e[s[n]]);
-        this.color = oi(u)
+        this.color = ri(u)
     }
-    if (jr[this.model])
+    if (Wr[this.model])
         for (r = Ke[this.model].channels, n = 0; n < r; n++) {
-            const o = jr[this.model][n];
+            const o = Wr[this.model][n];
             o && (this.color[n] = o(this.color[n]))
         }
     this.valpha = Math.max(0, Math.min(1, this.valpha)), Object.freeze && Object.freeze(this)
 }
 Ee.prototype = {
     toString() {
         return this.string()
     },
     toJSON() {
         return this[this.model]()
     },
     string(e) {
-        let t = this.model in hn.to ? this : this.rgb();
+        let t = this.model in pn.to ? this : this.rgb();
         t = t.round(typeof e == "number" ? e : 1);
         const n = t.valpha === 1 ? t.color : [...t.color, this.valpha];
-        return hn.to[t.model](n)
+        return pn.to[t.model](n)
     },
     percentString(e) {
         const t = this.rgb().round(typeof e == "number" ? e : 1),
             n = t.valpha === 1 ? t.color : [...t.color, this.valpha];
-        return hn.to.rgb.percent(n)
+        return pn.to.rgb.percent(n)
     },
     array() {
         return this.valpha === 1 ? [...this.color] : [...this.color, this.valpha]
     },
     object() {
         const e = {},
             {
@@ -8118,21 +8108,21 @@
     l: ze("lab", 0, Se(100)),
     a: ze("lab", 1),
     b: ze("lab", 2),
     keyword(e) {
         return e !== void 0 ? new Ee(e) : Ke[this.model].keyword(this.color)
     },
     hex(e) {
-        return e !== void 0 ? new Ee(e) : hn.to.hex(this.rgb().round().color)
+        return e !== void 0 ? new Ee(e) : pn.to.hex(this.rgb().round().color)
     },
     hexa(e) {
         if (e !== void 0) return new Ee(e);
         const t = this.rgb().round().color;
         let n = Math.round(this.valpha * 255).toString(16).toUpperCase();
-        return n.length === 1 && (n = "0" + n), hn.to.hex(t) + n
+        return n.length === 1 && (n = "0" + n), pn.to.hex(t) + n
     },
     rgbNumber() {
         const e = this.rgb().color;
         return (e[0] & 255) << 16 | (e[1] & 255) << 8 | e[2] & 255
     },
     luminosity() {
         const e = this.rgb().color,
@@ -8221,15 +8211,15 @@
     const {
         channels: t
     } = Ke[e];
     Ee.prototype[e] = function(...n) {
         return this.model === e ? new Ee(this) : n.length > 0 ? new Ee(n, e) : new Ee([...q0(Ke[this.model][e].raw(this.color)), this.valpha], e)
     }, Ee[e] = function(...n) {
         let r = n[0];
-        return typeof r == "number" && (r = oi(n, t)), new Ee(r, e)
+        return typeof r == "number" && (r = ri(n, t)), new Ee(r, e)
     }
 }
 
 function W0(e, t) {
     return Number(e.toFixed(t))
 }
 
@@ -8237,15 +8227,15 @@
     return function(t) {
         return W0(t, e)
     }
 }
 
 function ze(e, t, n) {
     e = Array.isArray(e) ? e : [e];
-    for (const r of e)(jr[r] || (jr[r] = []))[t] = n;
+    for (const r of e)(Wr[r] || (Wr[r] = []))[t] = n;
     return e = e[0],
         function(r) {
             let o;
             return r !== void 0 ? (n && (r = n(r)), o = this[e](), o.color[t] = r, o) : (o = this[e]().color[t], n && (o = n(o)), o)
         }
 }
 
@@ -8255,20 +8245,20 @@
     }
 }
 
 function q0(e) {
     return Array.isArray(e) ? e : [e]
 }
 
-function oi(e, t) {
+function ri(e, t) {
     for (let n = 0; n < t; n++) typeof e[n] != "number" && (e[n] = 0);
     return e
 }
 var K0 = Ee;
-const ys = vc(K0);
+const gs = yc(K0);
 if (!At) var At = {
     map: function(e, t) {
         var n = {};
         return t ? e.map(function(r, o) {
             return n.index = o, t.call(n, r)
         }) : e.slice()
     },
@@ -8503,18 +8493,18 @@
     }().quantize,
     tu = function(e) {
         this.canvas = document.createElement("canvas"), this.context = this.canvas.getContext("2d"), this.width = this.canvas.width = e.naturalWidth, this.height = this.canvas.height = e.naturalHeight, this.context.drawImage(e, 0, 0, this.width, this.height)
     };
 tu.prototype.getImageData = function() {
     return this.context.getImageData(0, 0, this.width, this.height)
 };
-var zn = function() {};
-zn.prototype.getColor = function(e, t) {
+var hn = function() {};
+hn.prototype.getColor = function(e, t) {
     return t === void 0 && (t = 10), this.getPalette(e, 5, t)[0]
-}, zn.prototype.getPalette = function(e, t, n) {
+}, hn.prototype.getPalette = function(e, t, n) {
     var r = function(u) {
             var c = u.colorCount,
                 l = u.quality;
             if (c !== void 0 && Number.isInteger(c)) {
                 if (c === 1) throw new Error("colorCount should be between 2 and 20. To get one color, call getColor() instead of getPalette()");
                 c = Math.max(c, 2), c = Math.min(c, 20)
             } else c = 10;
@@ -8529,34 +8519,34 @@
         o = new tu(e),
         a = function(u, c, l) {
             for (var d, m, f, _, p, b = u, T = [], v = 0; v < c; v += l) m = b[0 + (d = 4 * v)], f = b[d + 1], _ = b[d + 2], ((p = b[d + 3]) === void 0 || p >= 125) && (m > 250 && f > 250 && _ > 250 || T.push([m, f, _]));
             return T
         }(o.getImageData().data, o.width * o.height, r.quality),
         s = X0(a, r.colorCount);
     return s ? s.palette() : null
-}, zn.prototype.getColorFromUrl = function(e, t, n) {
+}, hn.prototype.getColorFromUrl = function(e, t, n) {
     var r = this,
         o = document.createElement("img");
     o.addEventListener("load", function() {
         var a = r.getPalette(o, 5, n);
         t(a[0], e)
     }), o.src = e
-}, zn.prototype.getImageData = function(e, t) {
+}, hn.prototype.getImageData = function(e, t) {
     var n = new XMLHttpRequest;
     n.open("GET", e, !0), n.responseType = "arraybuffer", n.onload = function() {
         if (this.status == 200) {
             var r = new Uint8Array(this.response);
             i = r.length;
             for (var o = new Array(i), a = 0; a < r.length; a++) o[a] = String.fromCharCode(r[a]);
             var s = o.join(""),
                 u = window.btoa(s);
             t("data:image/png;base64," + u)
         }
     }, n.send()
-}, zn.prototype.getColorAsync = function(e, t, n) {
+}, hn.prototype.getColorAsync = function(e, t, n) {
     var r = this;
     this.getImageData(e, function(o) {
         var a = document.createElement("img");
         a.addEventListener("load", function() {
             var s = r.getPalette(a, 5, n);
             t(s[0], this)
         }), a.src = o
@@ -8569,76 +8559,76 @@
             n = Math.floor((e - t * 3600) / 60),
             r = e - t * 3600 - n * 60;
         let o = t.toString(),
             a = n.toString(),
             s = r.toString();
         return t < 10 && (o = "0" + t), n < 10 && (a = "0" + n), r < 10 && (s = "0" + r), o === "00" ? a + ":" + s : o + ":" + a + ":" + s
     },
-    vs = function(e, t) {
+    ys = function(e, t) {
         return e ? e.length <= t ? e : e.slice(0, t) + "..." : ""
     },
     Ub = function(e, t) {
         return e ? t ? e.slice(0, t).map(n => n.name).join(" | ") : e.map(n => n.name).join(" | ") : ""
     },
     Wb = function(e, t) {
         let n = "";
         return e != null && e.name && (e != null && e.label) ? n = `${e.name}: ${t(e==null?void 0:e.label)}` : e != null && e.name ? n = e.name : e != null && e.label ? n = t(e == null ? void 0 : e.label) : n = e.path || "", n
     },
     jb = function(e, t = 26) {
-        return e ? e.type != Pc.GROUP && e.group_childs.length > 1 ? `${vs(e.display_name,t-3)} +${e.group_childs.length-1}` : vs(e.display_name, t) : ""
+        return e ? e.type != Pc.GROUP && e.group_childs.length > 1 ? `${ys(e.display_name,t-3)} +${e.group_childs.length-1}` : ys(e.display_name, t) : ""
     },
     qb = function(e) {
         const t = [];
         for (const n of (e == null ? void 0 : e.provider_mappings) || []) n.provider_domain.startsWith("filesystem") || n.provider_domain != "plex" && (t.filter(r => r.provider_domain == n.provider_domain).length || t.push(n));
         return console.log("getStreamingProviderMappings", t), t
     };
 
-function Mr(e) {
+function Er(e) {
     e = e.replace("#", ""), e.length === 3 && (e = e.split("").map(a => a + a).join(""));
     const t = parseInt(e.substr(0, 2), 16),
         n = parseInt(e.substr(2, 2), 16),
         r = parseInt(e.substr(4, 2), 16);
     return (.299 * t + .587 * n + .114 * r) / 255 > .7 ? "#000000" : "#FFFFFF"
 }
 
 function nu(e, t) {
-    const n = ys(e),
-        r = ys(t);
+    const n = gs(e),
+        r = gs(t);
     return n.contrast(r)
 }
 
-function Qi(e) {
+function Yi(e) {
     const [t, n, r] = e;
     return `#${t.toString(16).padStart(2,"0")}${n.toString(16).padStart(2,"0")}${r.toString(16).padStart(2,"0")}`
 }
 
 function $0(e) {
     let t = "",
         n = 0;
     return e.forEach(r => {
-        const o = Qi(r),
+        const o = Yi(r),
             a = nu("#000000", o);
         (a > n && a >= 7 || a > n && a >= n * .7) && (n = a, t = o)
     }), t
 }
 
 function Y0(e) {
     let t = "",
         n = 0;
     const r = 17.35;
     return e.forEach(o => {
-        const a = Qi(o),
+        const a = Yi(o),
             s = nu("#fff", a);
         r >= s && (s > n && s >= 7 || s > n && s >= n * .7) && (n = s, t = a)
     }), t
 }
 
 function Kb(e) {
-    const n = new zn().getPalette(e, 5),
-        r = n.map(o => Qi(o));
+    const n = new hn().getPalette(e, 5),
+        r = n.map(o => Yi(o));
     return {
         0: r[0],
         1: r[1],
         2: r[2],
         3: r[3],
         4: r[4],
         lightColor: $0(n),
@@ -8653,25 +8643,25 @@
             o = r[0],
             a = r[1],
             s = r[2];
         if (o) return a;
         if (s !== void 0) return s
     }
 }
-const Q0 = no({
+const Q0 = to({
     __name: "App",
     setup(e) {
         const t = o0();
         let n = t.themes.value.light,
             r = t.themes.value.dark;
         const o = function(c) {
-                n.colors.primary = c.lightColor || "#03a9f4", n.colors["on-primary"] = Mr(c.lightColor) || "#fff", n.colors.secondary = c.darkColor || "#ff9800", n.colors["on-secondary"] = Mr(c.darkColor) || "#fff", n.variables["medium-emphasis-opacity"] = 1, r.colors.primary = c.darkColor || "#0288d1", r.colors["on-primary"] = Mr(c.darkColor) || "#fff", r.colors.secondary = c.lightColor || "#ff9800", r.colors["on-secondary"] = Mr(c.lightColor) || "#fff", r.variables["medium-emphasis-opacity"] = 1
+                n.colors.primary = c.lightColor || "#03a9f4", n.colors["on-primary"] = Er(c.lightColor) || "#fff", n.colors.secondary = c.darkColor || "#ff9800", n.colors["on-secondary"] = Er(c.darkColor) || "#fff", n.variables["medium-emphasis-opacity"] = 1, r.colors.primary = c.darkColor || "#0288d1", r.colors["on-primary"] = Er(c.darkColor) || "#fff", r.colors.secondary = c.lightColor || "#ff9800", r.colors["on-secondary"] = Er(c.lightColor) || "#fff", r.variables["medium-emphasis-opacity"] = 1
             },
             a = re(() => {
-                if (ut.selectedPlayer) return Yo.queues[ut.selectedPlayer.active_source]
+                if (ut.selectedPlayer) return $o.queues[ut.selectedPlayer.active_source]
             }),
             s = re(() => {
                 if (a.value) return a.value.current_item
             });
 
         function u() {
             s.value ? o(ut.coverImageColorCode) : o({
@@ -8682,27 +8672,27 @@
         return xe(() => {
             var c;
             return (c = a.value) == null ? void 0 : c.display_name
         }, () => {
             u()
         }), xe(() => ut.coverImageColorCode, () => {
             u()
-        }), io(() => {
+        }), oo(() => {
             window.matchMedia("(prefers-color-scheme: dark)").addEventListener("change", l => {
                 const d = l.matches ? "dark" : "light";
                 t.global.name.value = d
             }), window.matchMedia && window.matchMedia("(prefers-color-scheme: dark)").matches && (t.global.name.value = "dark");
             let c = ""; {
                 const l = window.location;
                 c = l.origin + l.pathname
             }
-            Yo.initialize(c)
+            $o.initialize(c)
         }), (c, l) => {
             const d = ad("router-view");
-            return Vi(), Ui(d)
+            return Fi(), Vi(d)
         }
     }
 });
 const Z0 = Object.freeze({
         base: "#f44336",
         lighten5: "#ffebee",
         lighten4: "#ffcdd2",
@@ -8995,15 +8985,15 @@
         darken4: "#212121"
     }),
     zp = Object.freeze({
         black: "#000000",
         white: "#ffffff",
         transparent: "#ffffff00"
     }),
-    wr = Object.freeze({
+    Mr = Object.freeze({
         red: Z0,
         pink: J0,
         purple: ep,
         deepPurple: tp,
         indigo: np,
         blue: rp,
         lightBlue: op,
@@ -9048,39 +9038,39 @@
         },
         theme: {
             defaultTheme: "light",
             themes: {
                 light: {
                     dark: !1,
                     colors: {
-                        primary: wr.blue.base,
-                        accent: wr.blue.darken2
+                        primary: Mr.blue.base,
+                        accent: Mr.blue.darken2
                     }
                 },
                 dark: {
                     dark: !0,
                     colors: {
-                        primary: wr.blue.darken4,
-                        accent: wr.blue.lighten2
+                        primary: Mr.blue.darken4,
+                        accent: Mr.blue.lighten2
                     }
                 }
             }
         }
     }),
     yp = "modulepreload",
     vp = function(e, t) {
         return new URL(e, t).href
     },
-    Ts = {},
+    vs = {},
     pe = function(t, n, r) {
         if (!n || n.length === 0) return t();
         const o = document.getElementsByTagName("link");
         return Promise.all(n.map(a => {
-            if (a = vp(a, r), a in Ts) return;
-            Ts[a] = !0;
+            if (a = vp(a, r), a in vs) return;
+            vs[a] = !0;
             const s = a.endsWith(".css"),
                 u = s ? '[rel="stylesheet"]' : "";
             if (!!r)
                 for (let d = o.length - 1; d >= 0; d--) {
                     const m = o[d];
                     if (m.href === a && (!s || m.rel === "stylesheet")) return
                 } else if (document.querySelector(`link[href="${a}"]${u}`)) return;
@@ -9096,35 +9086,35 @@
         })
     };
 /*!
  * vue-router v4.2.4
  * (c) 2023 Eduardo San Martin Morote
  * @license MIT
  */
-const bn = typeof window < "u";
+const zn = typeof window < "u";
 
 function Tp(e) {
     return e.__esModule || e[Symbol.toStringTag] === "Module"
 }
 const ce = Object.assign;
 
-function Oo(e, t) {
+function Io(e, t) {
     const n = {};
     for (const r in t) {
         const o = t[r];
         n[r] = dt(o) ? o.map(e) : e(o)
     }
     return n
 }
-const Kn = () => {},
+const qn = () => {},
     dt = Array.isArray,
     Sp = /\/$/,
     Ap = e => e.replace(Sp, "");
 
-function Go(e, t, n = "/") {
+function Oo(e, t, n = "/") {
     let r, o = {},
         a = "",
         s = "";
     const u = t.indexOf("#");
     let c = t.indexOf("?");
     return u < c && u >= 0 && (c = -1), c > -1 && (r = t.slice(0, c), a = t.slice(c + 1, u > -1 ? u : t.length), o = e(a)), u > -1 && (r = r || t.slice(0, u), s = t.slice(u, t.length)), r = wp(r ?? t, n), {
         fullPath: r + (a && "?") + a + s,
@@ -9135,40 +9125,40 @@
 }
 
 function Pp(e, t) {
     const n = t.query ? e(t.query) : "";
     return t.path + (n && "?") + n + (t.hash || "")
 }
 
-function Ss(e, t) {
+function Ts(e, t) {
     return !t || !e.toLowerCase().startsWith(t.toLowerCase()) ? e : e.slice(t.length) || "/"
 }
 
 function Ep(e, t, n) {
     const r = t.matched.length - 1,
         o = n.matched.length - 1;
-    return r > -1 && r === o && Cn(t.matched[r], n.matched[o]) && ru(t.params, n.params) && e(t.query) === e(n.query) && t.hash === n.hash
+    return r > -1 && r === o && wn(t.matched[r], n.matched[o]) && ru(t.params, n.params) && e(t.query) === e(n.query) && t.hash === n.hash
 }
 
-function Cn(e, t) {
+function wn(e, t) {
     return (e.aliasOf || e) === (t.aliasOf || t)
 }
 
 function ru(e, t) {
     if (Object.keys(e).length !== Object.keys(t).length) return !1;
     for (const n in e)
         if (!Mp(e[n], t[n])) return !1;
     return !0
 }
 
 function Mp(e, t) {
-    return dt(e) ? As(e, t) : dt(t) ? As(t, e) : e === t
+    return dt(e) ? Ss(e, t) : dt(t) ? Ss(t, e) : e === t
 }
 
-function As(e, t) {
+function Ss(e, t) {
     return dt(t) ? e.length === t.length && e.every((n, r) => n === t[r]) : e.length === 1 && e[0] === t
 }
 
 function wp(e, t) {
     if (e.startsWith("/")) return e;
     if (!e) return t;
     const n = t.split("/"),
@@ -9179,26 +9169,26 @@
         s, u;
     for (s = 0; s < r.length; s++)
         if (u = r[s], u !== ".")
             if (u === "..") a > 1 && a--;
             else break;
     return n.slice(0, a).join("/") + "/" + r.slice(s - (s === r.length ? 1 : 0)).join("/")
 }
-var lr;
+var sr;
 (function(e) {
     e.pop = "pop", e.push = "push"
-})(lr || (lr = {}));
-var Xn;
+})(sr || (sr = {}));
+var Kn;
 (function(e) {
     e.back = "back", e.forward = "forward", e.unknown = ""
-})(Xn || (Xn = {}));
+})(Kn || (Kn = {}));
 
 function Cp(e) {
     if (!e)
-        if (bn) {
+        if (zn) {
             const t = document.querySelector("base");
             e = t && t.getAttribute("href") || "/", e = e.replace(/^\w+:\/\/[^\/]+/, "")
         } else e = "/";
     return e[0] !== "/" && e[0] !== "#" && (e = "/" + e), Ap(e)
 }
 const kp = /^[^#]+#/;
 
@@ -9211,15 +9201,15 @@
         r = e.getBoundingClientRect();
     return {
         behavior: t.behavior,
         left: r.left - n.left - (t.left || 0),
         top: r.top - n.top - (t.top || 0)
     }
 }
-const ho = () => ({
+const po = () => ({
     left: window.pageXOffset,
     top: window.pageYOffset
 });
 
 function Op(e) {
     let t;
     if ("el" in e) {
@@ -9228,41 +9218,41 @@
             o = typeof n == "string" ? r ? document.getElementById(n.slice(1)) : document.querySelector(n) : n;
         if (!o) return;
         t = Ip(o, e)
     } else t = e;
     "scrollBehavior" in document.documentElement.style ? window.scrollTo(t) : window.scrollTo(t.left != null ? t.left : window.pageXOffset, t.top != null ? t.top : window.pageYOffset)
 }
 
-function Ps(e, t) {
+function As(e, t) {
     return (history.state ? history.state.position - t : -1) + e
 }
-const ii = new Map;
+const oi = new Map;
 
 function Gp(e, t) {
-    ii.set(e, t)
+    oi.set(e, t)
 }
 
 function Rp(e) {
-    const t = ii.get(e);
-    return ii.delete(e), t
+    const t = oi.get(e);
+    return oi.delete(e), t
 }
 let Lp = () => location.protocol + "//" + location.host;
 
 function ou(e, t) {
     const {
         pathname: n,
         search: r,
         hash: o
     } = t, a = e.indexOf("#");
     if (a > -1) {
         let u = o.includes(e.slice(a)) ? e.slice(a).length : 1,
             c = o.slice(u);
-        return c[0] !== "/" && (c = "/" + c), Ss(c, "")
+        return c[0] !== "/" && (c = "/" + c), Ts(c, "")
     }
-    return Ss(n, e) + r + o
+    return Ts(n, e) + r + o
 }
 
 function Bp(e, t, n, r) {
     let o = [],
         a = [],
         s = null;
     const u = ({
@@ -9278,16 +9268,16 @@
                 return
             }
             T = b ? f.position - b.position : 0
         } else r(_);
         o.forEach(v => {
             v(n.value, p, {
                 delta: T,
-                type: lr.pop,
-                direction: T ? T > 0 ? Xn.forward : Xn.back : Xn.unknown
+                type: sr.pop,
+                direction: T ? T > 0 ? Kn.forward : Kn.back : Kn.unknown
             })
         })
     };
 
     function c() {
         s = n.value
     }
@@ -9302,15 +9292,15 @@
     }
 
     function d() {
         const {
             history: f
         } = window;
         f.state && f.replaceState(ce({}, f.state, {
-            scroll: ho()
+            scroll: po()
         }), "")
     }
 
     function m() {
         for (const f of a) f();
         a = [], window.removeEventListener("popstate", u), window.removeEventListener("beforeunload", d)
     }
@@ -9319,22 +9309,22 @@
     }), {
         pauseListeners: c,
         listen: l,
         destroy: m
     }
 }
 
-function Es(e, t, n, r = !1, o = !1) {
+function Ps(e, t, n, r = !1, o = !1) {
     return {
         back: e,
         current: t,
         forward: n,
         replaced: r,
         position: window.history.length,
-        scroll: o ? ho() : null
+        scroll: o ? po() : null
     }
 }
 
 function Np(e) {
     const {
         history: t,
         location: n
@@ -9359,27 +9349,27 @@
             t[d ? "replaceState" : "pushState"](l, "", f), o.value = l
         } catch (_) {
             console.error(_), n[d ? "replace" : "assign"](f)
         }
     }
 
     function s(c, l) {
-        const d = ce({}, t.state, Es(o.value.back, c, o.value.forward, !0), l, {
+        const d = ce({}, t.state, Ps(o.value.back, c, o.value.forward, !0), l, {
             position: o.value.position
         });
         a(c, d, !0), r.value = c
     }
 
     function u(c, l) {
         const d = ce({}, o.value, t.state, {
             forward: c,
-            scroll: ho()
+            scroll: po()
         });
         a(d.current, d, !0);
-        const m = ce({}, Es(r.value, c, null), {
+        const m = ce({}, Ps(r.value, c, null), {
             position: d.position + 1
         }, l);
         a(c, m, !1), r.value = c
     }
     return {
         location: r,
         state: o,
@@ -9430,30 +9420,30 @@
         hash: "",
         fullPath: "/",
         matched: [],
         meta: {},
         redirectedFrom: void 0
     },
     au = Symbol("");
-var Ms;
+var Es;
 (function(e) {
     e[e.aborted = 4] = "aborted", e[e.cancelled = 8] = "cancelled", e[e.duplicated = 16] = "duplicated"
-})(Ms || (Ms = {}));
+})(Es || (Es = {}));
 
-function kn(e, t) {
+function Cn(e, t) {
     return ce(new Error, {
         type: e,
         [au]: !0
     }, t)
 }
 
 function vt(e, t) {
     return e instanceof Error && au in e && (t == null || !!(e.type & t))
 }
-const ws = "[^/]+?",
+const Ms = "[^/]+?",
     Vp = {
         sensitive: !1,
         strict: !1,
         start: !0,
         end: !0
     },
     Up = /[.+*?^${}()[\]/\\]/g;
@@ -9478,16 +9468,16 @@
                     regexp: v
                 } = f;
                 a.push({
                     name: p,
                     repeatable: b,
                     optional: T
                 });
-                const A = v || ws;
-                if (A !== ws) {
+                const A = v || Ms;
+                if (A !== Ms) {
                     _ += 10;
                     try {
                         new RegExp(`(${A})`)
                     } catch (P) {
                         throw new Error(`Invalid custom RegExp for param "${p}" (${A}): ` + P.message)
                     }
                 }
@@ -9565,21 +9555,21 @@
         o = t.score;
     for (; n < r.length && n < o.length;) {
         const a = jp(r[n], o[n]);
         if (a) return a;
         n++
     }
     if (Math.abs(o.length - r.length) === 1) {
-        if (Cs(r)) return 1;
-        if (Cs(o)) return -1
+        if (ws(r)) return 1;
+        if (ws(o)) return -1
     }
     return o.length - r.length
 }
 
-function Cs(e) {
+function ws(e) {
     const t = e[e.length - 1];
     return e.length > 0 && t[t.length - 1] < 0
 }
 const Kp = {
         type: 0,
         value: ""
     },
@@ -9664,29 +9654,29 @@
         });
     return t && !o.record.aliasOf == !t.record.aliasOf && t.children.push(o), o
 }
 
 function Qp(e, t) {
     const n = [],
         r = new Map;
-    t = Is({
+    t = Ds({
         strict: !1,
         end: !0,
         sensitive: !1
     }, t);
 
     function o(d) {
         return r.get(d)
     }
 
     function a(d, m, f) {
         const _ = !f,
             p = Zp(d);
         p.aliasOf = f && f.record;
-        const b = Is(t, d),
+        const b = Ds(t, d),
             T = [p];
         if ("alias" in d) {
             const I = typeof d.alias == "string" ? [d.alias] : d.alias;
             for (const P of I) T.push(ce({}, p, {
                 components: f ? f.record.components : p.components,
                 path: P,
                 aliasOf: f ? f.record : p
@@ -9698,23 +9688,23 @@
                 path: P
             } = I;
             if (m && P[0] !== "/") {
                 const M = m.record.path,
                     N = M[M.length - 1] === "/" ? "" : "/";
                 I.path = m.record.path + (P && N + P)
             }
-            if (v = Yp(I, m, b), f ? f.alias.push(v) : (A = A || v, A !== v && A.alias.push(v), _ && d.name && !Ds(v) && s(d.name)), p.children) {
+            if (v = Yp(I, m, b), f ? f.alias.push(v) : (A = A || v, A !== v && A.alias.push(v), _ && d.name && !ks(v) && s(d.name)), p.children) {
                 const M = p.children;
                 for (let N = 0; N < M.length; N++) a(M[N], v, f && f.children[N])
             }
             f = f || v, (v.record.components && Object.keys(v.record.components).length || v.record.name || v.record.redirect) && c(v)
         }
         return A ? () => {
             s(A)
-        } : Kn
+        } : qn
     }
 
     function s(d) {
         if (iu(d)) {
             const m = r.get(d);
             m && (r.delete(d), n.splice(n.indexOf(m), 1), m.children.forEach(s), m.alias.forEach(s))
         } else {
@@ -9726,28 +9716,28 @@
     function u() {
         return n
     }
 
     function c(d) {
         let m = 0;
         for (; m < n.length && qp(d, n[m]) >= 0 && (d.record.path !== n[m].record.path || !su(d, n[m]));) m++;
-        n.splice(m, 0, d), d.record.name && !Ds(d) && r.set(d.record.name, d)
+        n.splice(m, 0, d), d.record.name && !ks(d) && r.set(d.record.name, d)
     }
 
     function l(d, m) {
         let f, _ = {},
             p, b;
         if ("name" in d && d.name) {
-            if (f = r.get(d.name), !f) throw kn(1, {
+            if (f = r.get(d.name), !f) throw Cn(1, {
                 location: d
             });
-            b = f.record.name, _ = ce(ks(m.params, f.keys.filter(A => !A.optional).map(A => A.name)), d.params && ks(d.params, f.keys.map(A => A.name))), p = f.stringify(_)
+            b = f.record.name, _ = ce(Cs(m.params, f.keys.filter(A => !A.optional).map(A => A.name)), d.params && Cs(d.params, f.keys.map(A => A.name))), p = f.stringify(_)
         } else if ("path" in d) p = d.path, f = n.find(A => A.re.test(p)), f && (_ = f.parse(p), b = f.record.name);
         else {
-            if (f = m.name ? r.get(m.name) : n.find(A => A.re.test(m.path)), !f) throw kn(1, {
+            if (f = m.name ? r.get(m.name) : n.find(A => A.re.test(m.path)), !f) throw Cn(1, {
                 location: d,
                 currentLocation: m
             });
             b = f.record.name, _ = ce({}, m.params, d.params), p = f.stringify(_)
         }
         const T = [];
         let v = f;
@@ -9765,15 +9755,15 @@
         resolve: l,
         removeRoute: s,
         getRoutes: u,
         getRecordMatcher: o
     }
 }
 
-function ks(e, t) {
+function Cs(e, t) {
     const n = {};
     for (const r of t) r in e && (n[r] = e[r]);
     return n
 }
 
 function Zp(e) {
     return {
@@ -9800,27 +9790,27 @@
         n = e.props || !1;
     if ("component" in e) t.default = n;
     else
         for (const r in e.components) t[r] = typeof n == "object" ? n[r] : n;
     return t
 }
 
-function Ds(e) {
+function ks(e) {
     for (; e;) {
         if (e.record.aliasOf) return !0;
         e = e.parent
     }
     return !1
 }
 
 function eh(e) {
     return e.reduce((t, n) => ce(t, n.meta), {})
 }
 
-function Is(e, t) {
+function Ds(e, t) {
     const n = {};
     for (const r in e) n[r] = r in t ? t[r] : e[r];
     return n
 }
 
 function su(e, t) {
     return t.children.some(n => n === e || su(e, n))
@@ -9836,70 +9826,70 @@
     uu = /%5E/g,
     sh = /%60/g,
     mu = /%7B/g,
     lh = /%7C/g,
     du = /%7D/g,
     ch = /%20/g;
 
-function Zi(e) {
+function Qi(e) {
     return encodeURI("" + e).replace(lh, "|").replace(ih, "[").replace(ah, "]")
 }
 
 function uh(e) {
-    return Zi(e).replace(mu, "{").replace(du, "}").replace(uu, "^")
+    return Qi(e).replace(mu, "{").replace(du, "}").replace(uu, "^")
 }
 
-function ai(e) {
-    return Zi(e).replace(cu, "%2B").replace(ch, "+").replace(lu, "%23").replace(th, "%26").replace(sh, "`").replace(mu, "{").replace(du, "}").replace(uu, "^")
+function ii(e) {
+    return Qi(e).replace(cu, "%2B").replace(ch, "+").replace(lu, "%23").replace(th, "%26").replace(sh, "`").replace(mu, "{").replace(du, "}").replace(uu, "^")
 }
 
 function mh(e) {
-    return ai(e).replace(rh, "%3D")
+    return ii(e).replace(rh, "%3D")
 }
 
 function dh(e) {
-    return Zi(e).replace(lu, "%23").replace(oh, "%3F")
+    return Qi(e).replace(lu, "%23").replace(oh, "%3F")
 }
 
 function fh(e) {
     return e == null ? "" : dh(e).replace(nh, "%2F")
 }
 
-function qr(e) {
+function jr(e) {
     try {
         return decodeURIComponent("" + e)
     } catch {}
     return "" + e
 }
 
 function _h(e) {
     const t = {};
     if (e === "" || e === "?") return t;
     const r = (e[0] === "?" ? e.slice(1) : e).split("&");
     for (let o = 0; o < r.length; ++o) {
         const a = r[o].replace(cu, " "),
             s = a.indexOf("="),
-            u = qr(s < 0 ? a : a.slice(0, s)),
-            c = s < 0 ? null : qr(a.slice(s + 1));
+            u = jr(s < 0 ? a : a.slice(0, s)),
+            c = s < 0 ? null : jr(a.slice(s + 1));
         if (u in t) {
             let l = t[u];
             dt(l) || (l = t[u] = [l]), l.push(c)
         } else t[u] = c
     }
     return t
 }
 
-function Os(e) {
+function Is(e) {
     let t = "";
     for (let n in e) {
         const r = e[n];
         if (n = mh(n), r == null) {
             r !== void 0 && (t += (t.length ? "&" : "") + n);
             continue
-        }(dt(r) ? r.map(a => a && ai(a)) : [r && ai(r)]).forEach(a => {
+        }(dt(r) ? r.map(a => a && ii(a)) : [r && ii(r)]).forEach(a => {
             a !== void 0 && (t += (t.length ? "&" : "") + n, a != null && (t += "=" + a))
         })
     }
     return t
 }
 
 function ph(e) {
@@ -9907,20 +9897,20 @@
     for (const n in e) {
         const r = e[n];
         r !== void 0 && (t[n] = dt(r) ? r.map(o => o == null ? null : "" + o) : r == null ? r : "" + r)
     }
     return t
 }
 const hh = Symbol(""),
-    Gs = Symbol(""),
-    zo = Symbol(""),
+    Os = Symbol(""),
+    ho = Symbol(""),
     fu = Symbol(""),
-    si = Symbol("");
+    ai = Symbol("");
 
-function Nn() {
+function Bn() {
     let e = [];
 
     function t(r) {
         return e.push(r), () => {
             const o = e.indexOf(r);
             o > -1 && e.splice(o, 1)
         }
@@ -9936,29 +9926,29 @@
     }
 }
 
 function Ot(e, t, n, r, o) {
     const a = r && (r.enterCallbacks[o] = r.enterCallbacks[o] || []);
     return () => new Promise((s, u) => {
         const c = m => {
-                m === !1 ? u(kn(4, {
+                m === !1 ? u(Cn(4, {
                     from: n,
                     to: t
-                })) : m instanceof Error ? u(m) : Fp(m) ? u(kn(2, {
+                })) : m instanceof Error ? u(m) : Fp(m) ? u(Cn(2, {
                     from: t,
                     to: m
                 })) : (a && r.enterCallbacks[o] === a && typeof m == "function" && a.push(m), s())
             },
             l = e.call(r && r.instances[o], t, n, c);
         let d = Promise.resolve(l);
         e.length < 3 && (d = d.then(c)), d.catch(m => u(m))
     })
 }
 
-function Ro(e, t, n, r) {
+function Go(e, t, n, r) {
     const o = [];
     for (const a of e)
         for (const s in a.components) {
             let u = a.components[s];
             if (!(t !== "beforeRouteEnter" && !a.instances[s]))
                 if (zh(u)) {
                     const l = (u.__vccOpts || u)[t];
@@ -9977,45 +9967,45 @@
     return o
 }
 
 function zh(e) {
     return typeof e == "object" || "displayName" in e || "props" in e || "__vccOpts" in e
 }
 
-function Rs(e) {
-    const t = ke(zo),
+function Gs(e) {
+    const t = ke(ho),
         n = ke(fu),
         r = re(() => t.resolve(lt(e.to))),
         o = re(() => {
             const {
                 matched: c
             } = r.value, {
                 length: l
             } = c, d = c[l - 1], m = n.matched;
             if (!d || !m.length) return -1;
-            const f = m.findIndex(Cn.bind(null, d));
+            const f = m.findIndex(wn.bind(null, d));
             if (f > -1) return f;
-            const _ = Ls(c[l - 2]);
-            return l > 1 && Ls(d) === _ && m[m.length - 1].path !== _ ? m.findIndex(Cn.bind(null, c[l - 2])) : f
+            const _ = Rs(c[l - 2]);
+            return l > 1 && Rs(d) === _ && m[m.length - 1].path !== _ ? m.findIndex(wn.bind(null, c[l - 2])) : f
         }),
         a = re(() => o.value > -1 && vh(n.params, r.value.params)),
         s = re(() => o.value > -1 && o.value === n.matched.length - 1 && ru(n.params, r.value.params));
 
     function u(c = {}) {
-        return yh(c) ? t[lt(e.replace) ? "replace" : "push"](lt(e.to)).catch(Kn) : Promise.resolve()
+        return yh(c) ? t[lt(e.replace) ? "replace" : "push"](lt(e.to)).catch(qn) : Promise.resolve()
     }
     return {
         route: r,
         href: re(() => r.value.href),
         isActive: a,
         isExactActive: s,
         navigate: u
     }
 }
-const bh = no({
+const bh = to({
         name: "RouterLink",
         compatConfig: {
             MODE: 3
         },
         props: {
             to: {
                 type: [String, Object],
@@ -10026,25 +10016,25 @@
             exactActiveClass: String,
             custom: Boolean,
             ariaCurrentValue: {
                 type: String,
                 default: "page"
             }
         },
-        useLink: Rs,
+        useLink: Gs,
         setup(e, {
             slots: t
         }) {
-            const n = Xe(Rs(e)),
+            const n = Xe(Gs(e)),
                 {
                     options: r
-                } = ke(zo),
+                } = ke(ho),
                 o = re(() => ({
-                    [Bs(e.activeClass, r.linkActiveClass, "router-link-active")]: n.isActive,
-                    [Bs(e.exactActiveClass, r.linkExactActiveClass, "router-link-exact-active")]: n.isExactActive
+                    [Ls(e.activeClass, r.linkActiveClass, "router-link-active")]: n.isActive,
+                    [Ls(e.exactActiveClass, r.linkExactActiveClass, "router-link-exact-active")]: n.isExactActive
                 }));
             return () => {
                 const a = t.default && t.default(n);
                 return e.custom ? a : rn("a", {
                     "aria-current": n.isExactActive ? e.ariaCurrentValue : null,
                     href: n.href,
                     onClick: n.navigate,
@@ -10072,19 +10062,19 @@
         if (typeof r == "string") {
             if (r !== o) return !1
         } else if (!dt(o) || o.length !== r.length || r.some((a, s) => a !== o[s])) return !1
     }
     return !0
 }
 
-function Ls(e) {
+function Rs(e) {
     return e ? e.aliasOf ? e.aliasOf.path : e.path : ""
 }
-const Bs = (e, t, n) => e ?? t ?? n,
-    Th = no({
+const Ls = (e, t, n) => e ?? t ?? n,
+    Th = to({
         name: "RouterView",
         inheritAttrs: !1,
         props: {
             name: {
                 type: String,
                 default: "default"
             },
@@ -10093,80 +10083,80 @@
         compatConfig: {
             MODE: 3
         },
         setup(e, {
             attrs: t,
             slots: n
         }) {
-            const r = ke(si),
+            const r = ke(ai),
                 o = re(() => e.route || r.value),
-                a = ke(Gs, 0),
+                a = ke(Os, 0),
                 s = re(() => {
                     let l = lt(a);
                     const {
                         matched: d
                     } = o.value;
                     let m;
                     for (;
                         (m = d[l]) && !m.components;) l++;
                     return l
                 }),
                 u = re(() => o.value.matched[s.value]);
-            Pn(Gs, re(() => s.value + 1)), Pn(hh, u), Pn(si, o);
+            An(Os, re(() => s.value + 1)), An(hh, u), An(ai, o);
             const c = Me();
             return xe(() => [c.value, u.value, e.name], ([l, d, m], [f, _, p]) => {
-                d && (d.instances[m] = l, _ && _ !== d && l && l === f && (d.leaveGuards.size || (d.leaveGuards = _.leaveGuards), d.updateGuards.size || (d.updateGuards = _.updateGuards))), l && d && (!_ || !Cn(d, _) || !f) && (d.enterCallbacks[m] || []).forEach(b => b(l))
+                d && (d.instances[m] = l, _ && _ !== d && l && l === f && (d.leaveGuards.size || (d.leaveGuards = _.leaveGuards), d.updateGuards.size || (d.updateGuards = _.updateGuards))), l && d && (!_ || !wn(d, _) || !f) && (d.enterCallbacks[m] || []).forEach(b => b(l))
             }, {
                 flush: "post"
             }), () => {
                 const l = o.value,
                     d = e.name,
                     m = u.value,
                     f = m && m.components[d];
-                if (!f) return Ns(n.default, {
+                if (!f) return Bs(n.default, {
                     Component: f,
                     route: l
                 });
                 const _ = m.props[d],
                     p = _ ? _ === !0 ? l.params : typeof _ == "function" ? _(l) : _ : null,
                     T = rn(f, ce({}, p, t, {
                         onVnodeUnmounted: v => {
                             v.component.isUnmounted && (m.instances[d] = null)
                         },
                         ref: c
                     }));
-                return Ns(n.default, {
+                return Bs(n.default, {
                     Component: T,
                     route: l
                 }) || T
             }
         }
     });
 
-function Ns(e, t) {
+function Bs(e, t) {
     if (!e) return null;
     const n = e(t);
     return n.length === 1 ? n[0] : n
 }
 const Sh = Th;
 
 function Ah(e) {
     const t = Qp(e.routes, e),
         n = e.parseQuery || _h,
-        r = e.stringifyQuery || Os,
+        r = e.stringifyQuery || Is,
         o = e.history,
-        a = Nn(),
-        s = Nn(),
-        u = Nn(),
+        a = Bn(),
+        s = Bn(),
+        u = Bn(),
         c = Jt(kt);
     let l = kt;
-    bn && e.scrollBehavior && "scrollRestoration" in history && (history.scrollRestoration = "manual");
-    const d = Oo.bind(null, w => "" + w),
-        m = Oo.bind(null, fh),
-        f = Oo.bind(null, qr);
+    zn && e.scrollBehavior && "scrollRestoration" in history && (history.scrollRestoration = "manual");
+    const d = Io.bind(null, w => "" + w),
+        m = Io.bind(null, fh),
+        f = Io.bind(null, jr);
 
     function _(w, H) {
         let R, q;
         return iu(w) ? (R = t.getRecordMatcher(w), q = H) : q = w, t.addRoute(q, R)
     }
 
     function p(w) {
@@ -10180,29 +10170,29 @@
 
     function T(w) {
         return !!t.getRecordMatcher(w)
     }
 
     function v(w, H) {
         if (H = ce({}, H || c.value), typeof w == "string") {
-            const g = Go(n, w, H.path),
+            const g = Oo(n, w, H.path),
                 E = t.resolve({
                     path: g.path
                 }, H),
                 k = o.createHref(g.fullPath);
             return ce(g, E, {
                 params: f(E.params),
-                hash: qr(g.hash),
+                hash: jr(g.hash),
                 redirectedFrom: void 0,
                 href: k
             })
         }
         let R;
         if ("path" in w) R = ce({}, w, {
-            path: Go(n, w.path, H.path).path
+            path: Oo(n, w.path, H.path).path
         });
         else {
             const g = ce({}, w.params);
             for (const E in g) g[E] == null && delete g[E];
             R = ce({}, w, {
                 params: m(g)
             }), H.params = m(H.params)
@@ -10214,27 +10204,27 @@
                 hash: uh(se),
                 path: q.path
             })),
             z = o.createHref(h);
         return ce({
             fullPath: h,
             hash: se,
-            query: r === Os ? ph(w.query) : w.query || {}
+            query: r === Is ? ph(w.query) : w.query || {}
         }, q, {
             redirectedFrom: void 0,
             href: z
         })
     }
 
     function A(w) {
-        return typeof w == "string" ? Go(n, w, c.value.path) : ce({}, w)
+        return typeof w == "string" ? Oo(n, w, c.value.path) : ce({}, w)
     }
 
     function I(w, H) {
-        if (l !== w) return kn(8, {
+        if (l !== w) return Cn(8, {
             from: H,
             to: w
         })
     }
 
     function P(w) {
         return j(w)
@@ -10274,15 +10264,15 @@
             state: typeof g == "object" ? ce({}, se, g.state) : se,
             force: h,
             replace: z
         }), H || R);
         const E = R;
         E.redirectedFrom = H;
         let k;
-        return !h && Ep(r, q, R) && (k = kn(16, {
+        return !h && Ep(r, q, R) && (k = Cn(16, {
             to: E,
             from: q
         }), Qe(q, q, !0, !1)), (k ? Promise.resolve(k) : $(E, q)).catch(D => vt(D) ? vt(D, 2) ? D : ft(D) : oe(D, E, q)).then(D => {
             if (D) {
                 if (vt(D, 2)) return j(ce({
                     replace: z
                 }, A(D.to), {
@@ -10303,81 +10293,81 @@
         const H = Mt.values().next().value;
         return H && typeof H.runWithContext == "function" ? H.runWithContext(w) : w()
     }
 
     function $(w, H) {
         let R;
         const [q, se, h] = Ph(w, H);
-        R = Ro(q.reverse(), "beforeRouteLeave", w, H);
+        R = Go(q.reverse(), "beforeRouteLeave", w, H);
         for (const g of q) g.leaveGuards.forEach(E => {
             R.push(Ot(E, w, H))
         });
         const z = L.bind(null, w, H);
         return R.push(z), Pe(R).then(() => {
             R = [];
             for (const g of a.list()) R.push(Ot(g, w, H));
             return R.push(z), Pe(R)
         }).then(() => {
-            R = Ro(se, "beforeRouteUpdate", w, H);
+            R = Go(se, "beforeRouteUpdate", w, H);
             for (const g of se) g.updateGuards.forEach(E => {
                 R.push(Ot(E, w, H))
             });
             return R.push(z), Pe(R)
         }).then(() => {
             R = [];
             for (const g of h)
                 if (g.beforeEnter)
                     if (dt(g.beforeEnter))
                         for (const E of g.beforeEnter) R.push(Ot(E, w, H));
                     else R.push(Ot(g.beforeEnter, w, H));
             return R.push(z), Pe(R)
-        }).then(() => (w.matched.forEach(g => g.enterCallbacks = {}), R = Ro(h, "beforeRouteEnter", w, H), R.push(z), Pe(R))).then(() => {
+        }).then(() => (w.matched.forEach(g => g.enterCallbacks = {}), R = Go(h, "beforeRouteEnter", w, H), R.push(z), Pe(R))).then(() => {
             R = [];
             for (const g of s.list()) R.push(Ot(g, w, H));
             return R.push(z), Pe(R)
         }).catch(g => vt(g, 8) ? g : Promise.reject(g))
     }
 
     function Y(w, H, R) {
         u.list().forEach(q => X(() => q(w, H, R)))
     }
 
     function x(w, H, R, q, se) {
         const h = I(w, H);
         if (h) return h;
         const z = H === kt,
-            g = bn ? history.state : {};
+            g = zn ? history.state : {};
         R && (q || z ? o.replace(w.fullPath, ce({
             scroll: z && g && g.scroll
         }, se)) : o.push(w.fullPath, se)), c.value = w, Qe(w, H, R, z), ft()
     }
     let te;
 
     function De() {
         te || (te = o.listen((w, H, R) => {
             if (!an.listening) return;
             const q = v(w),
                 se = N(q);
             if (se) {
                 j(ce(se, {
                     replace: !0
-                }), q).catch(Kn);
+                }), q).catch(qn);
                 return
             }
             l = q;
             const h = c.value;
-            bn && Gp(Ps(h.fullPath, R.delta), ho()), $(q, h).catch(z => vt(z, 12) ? z : vt(z, 2) ? (j(z.to, q).then(g => {
-                vt(g, 20) && !R.delta && R.type === lr.pop && o.go(-1, !1)
-            }).catch(Kn), Promise.reject()) : (R.delta && o.go(-R.delta, !1), oe(z, q, h))).then(z => {
-                z = z || x(q, h, !1), z && (R.delta && !vt(z, 8) ? o.go(-R.delta, !1) : R.type === lr.pop && vt(z, 20) && o.go(-1, !1)), Y(q, h, z)
-            }).catch(Kn)
+            zn && Gp(As(h.fullPath, R.delta), po()), $(q, h).catch(z => vt(z, 12) ? z : vt(z, 2) ? (j(z.to, q).then(g => {
+                vt(g, 20) && !R.delta && R.type === sr.pop && o.go(-1, !1)
+            }).catch(qn), Promise.reject()) : (R.delta && o.go(-R.delta, !1), oe(z, q, h))).then(z => {
+                z = z || x(q, h, !1), z && (R.delta && !vt(z, 8) ? o.go(-R.delta, !1) : R.type === sr.pop && vt(z, 20) && o.go(-1, !1)), Y(q, h, z)
+            }).catch(qn)
         }))
     }
-    let ot = Nn(),
-        _e = Nn(),
+    let ot = Bn(),
+        _e = Bn(),
         ne;
 
     function oe(w, H, R) {
         ft(w);
         const q = _e.list();
         return q.length ? q.forEach(se => se(w, H, R)) : console.error(w), Promise.reject(w)
     }
@@ -10392,17 +10382,17 @@
         return ne || (ne = !w, De(), ot.list().forEach(([H, R]) => w ? R(w) : H()), ot.reset()), w
     }
 
     function Qe(w, H, R, q) {
         const {
             scrollBehavior: se
         } = e;
-        if (!bn || !se) return Promise.resolve();
-        const h = !R && Rp(Ps(w.fullPath, 0)) || (q || !R) && history.state && history.state.scroll || null;
-        return Ii().then(() => se(w, H, h)).then(z => z && Op(z)).catch(z => oe(z, w, H))
+        if (!zn || !se) return Promise.resolve();
+        const h = !R && Rp(As(w.fullPath, 0)) || (q || !R) && history.state && history.state.scroll || null;
+        return Di().then(() => se(w, H, h)).then(z => z && Op(z)).catch(z => oe(z, w, H))
     }
     const Ge = w => o.go(w);
     let Ft;
     const Mt = new Set,
         an = {
             currentRoute: c,
             listening: !0,
@@ -10423,21 +10413,21 @@
             onError: _e.add,
             isReady: it,
             install(w) {
                 const H = this;
                 w.component("RouterLink", gh), w.component("RouterView", Sh), w.config.globalProperties.$router = H, Object.defineProperty(w.config.globalProperties, "$route", {
                     enumerable: !0,
                     get: () => lt(c)
-                }), bn && !Ft && c.value === kt && (Ft = !0, P(o.location).catch(se => {}));
+                }), zn && !Ft && c.value === kt && (Ft = !0, P(o.location).catch(se => {}));
                 const R = {};
                 for (const se in kt) Object.defineProperty(R, se, {
                     get: () => c.value[se],
                     enumerable: !0
                 });
-                w.provide(zo, H), w.provide(fu, Cl(R)), w.provide(si, c);
+                w.provide(ho, H), w.provide(fu, wl(R)), w.provide(ai, c);
                 const q = w.unmount;
                 Mt.add(w), w.unmount = function() {
                     Mt.delete(w), Mt.size < 1 && (l = kt, te && te(), te = null, c.value = kt, Ft = !1, ne = !1), q()
                 }
             }
         };
 
@@ -10450,145 +10440,145 @@
 function Ph(e, t) {
     const n = [],
         r = [],
         o = [],
         a = Math.max(t.matched.length, e.matched.length);
     for (let s = 0; s < a; s++) {
         const u = t.matched[s];
-        u && (e.matched.find(l => Cn(l, u)) ? r.push(u) : n.push(u));
+        u && (e.matched.find(l => wn(l, u)) ? r.push(u) : n.push(u));
         const c = e.matched[s];
-        c && (t.matched.find(l => Cn(l, c)) || o.push(c))
+        c && (t.matched.find(l => wn(l, c)) || o.push(c))
     }
     return [n, r, o]
 }
 
 function $b() {
-    return ke(zo)
+    return ke(ho)
 }
 const Eh = [{
         path: "/",
-        component: () => pe(() => import("./Default-27a728f1.js"), ["./Default-27a728f1.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./layout-4499d5bc.js", "./Button-59559304.js", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-15e2fa72.css", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VExpansionPanel-67038b00.js", "./VExpansionPanel-16e67e58.css", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./Default-8766b49d.css"], import.meta.url),
+        component: () => pe(() => import("./Default-4e51f0b8.js"), ["./Default-4e51f0b8.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./layout-b0232ef9.js", "./Button-4a781169.js", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-15e2fa72.css", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VExpansionPanel-75456689.js", "./VExpansionPanel-16e67e58.css", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./Default-8766b49d.css"], import.meta.url),
         children: [{
             path: "",
             redirect: "/home",
             name: "homeredirect"
         }, {
             path: "/home",
             name: "home",
-            component: () => pe(() => import("./HomeView-6873693d.js"), ["./HomeView-6873693d.js", "./VRow-e8f3e51e.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VGrid-b9c72806.css", "./VCard-138864fc.js", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VCard-103d8462.css", "./HomeView-f559b858.css"], import.meta.url),
+            component: () => pe(() => import("./HomeView-af5707e7.js"), ["./HomeView-af5707e7.js", "./VRow-74a0e5a5.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VGrid-b9c72806.css", "./VCard-f3e11b51.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VCard-103d8462.css", "./HomeView-f559b858.css"], import.meta.url),
             props: !0
         }, {
             path: "/search",
             name: "search",
-            component: () => pe(() => import("./Search-b8c39f87.js"), ["./Search-b8c39f87.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./VRow-e8f3e51e.js", "./VSpacer-bdf2f653.js", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./Search-f31ee239.js"), ["./Search-f31ee239.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./VRow-74a0e5a5.js", "./VSpacer-159b0383.js", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/browse",
             name: "browse",
-            component: () => pe(() => import("./BrowseView-d63a1e11.js"), ["./BrowseView-d63a1e11.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./BrowseView-457188ac.js"), ["./BrowseView-457188ac.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: e => ({
                 path: e.query.path
             })
         }, {
             path: "/artists",
             name: "artists",
-            component: () => pe(() => import("./LibraryArtists-be1957cb.js"), ["./LibraryArtists-be1957cb.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryArtists-225ce0c1.js"), ["./LibraryArtists-225ce0c1.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/tracks",
             name: "tracks",
-            component: () => pe(() => import("./LibraryTracks-d64430e5.js"), ["./LibraryTracks-d64430e5.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryTracks-5a540fa3.js"), ["./LibraryTracks-5a540fa3.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/albums",
             name: "albums",
-            component: () => pe(() => import("./LibraryAlbums-ea4898eb.js"), ["./LibraryAlbums-ea4898eb.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryAlbums-757b8aa2.js"), ["./LibraryAlbums-757b8aa2.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/playlists",
             name: "playlists",
-            component: () => pe(() => import("./LibraryPlaylists-a9b54924.js"), ["./LibraryPlaylists-a9b54924.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryPlaylists-4ffdc19f.js"), ["./LibraryPlaylists-4ffdc19f.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/radios",
             name: "radios",
-            component: () => pe(() => import("./LibraryRadios-996c89ba.js"), ["./LibraryRadios-996c89ba.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./LibraryRadios-a948d358.js"), ["./LibraryRadios-a948d358.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/artists/:provider/:itemId",
             name: "artist",
-            component: () => pe(() => import("./ArtistDetails-7bca6a8e.js"), ["./ArtistDetails-7bca6a8e.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js", "./layout-4499d5bc.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./ArtistDetails-7c7516d2.js"), ["./ArtistDetails-7c7516d2.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/albums/:provider/:itemId",
             name: "album",
-            component: () => pe(() => import("./AlbumDetails-343f22cb.js"), ["./AlbumDetails-343f22cb.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js", "./layout-4499d5bc.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./AlbumDetails-55ac33a4.js"), ["./AlbumDetails-55ac33a4.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/tracks/:provider/:itemId",
             name: "track",
-            component: () => pe(() => import("./TrackDetails-71587bd7.js"), ["./TrackDetails-71587bd7.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js", "./layout-4499d5bc.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./TrackDetails-ca02e9b2.js"), ["./TrackDetails-ca02e9b2.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: e => ({
                 ...e.params,
                 ...e.query
             })
         }, {
             path: "/radios/:provider/:itemId",
             name: "radio",
-            component: () => pe(() => import("./RadioDetails-6f742445.js"), ["./RadioDetails-6f742445.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js", "./layout-4499d5bc.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./RadioDetails-71dc877e.js"), ["./RadioDetails-71dc877e.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/playlists/:provider/:itemId",
             name: "playlist",
-            component: () => pe(() => import("./PlaylistDetails-09b11191.js"), ["./PlaylistDetails-09b11191.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js", "./PanelviewItem-14a6b77a.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VSpacer-bdf2f653.js", "./VBadge-9fa94f29.js", "./VBadge-9c063078.css", "./VRow-e8f3e51e.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js", "./layout-4499d5bc.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
+            component: () => pe(() => import("./PlaylistDetails-f8a1c191.js"), ["./PlaylistDetails-f8a1c191.js", "./ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js", "./PanelviewItem-14a6b77a.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VSpacer-159b0383.js", "./VBadge-12aff0c7.js", "./VBadge-9c063078.css", "./VRow-74a0e5a5.js", "./ItemsListing-7290acd0.css", "./vue-virtual-scroller-4d71315f.css", "./InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js", "./layout-b0232ef9.js", "./InfoHeader-32cd2df9.css"], import.meta.url),
             props: !0
         }, {
             path: "/playerqueue",
             name: "playerqueue",
-            component: () => pe(() => import("./PlayerQueue-29876489.js"), ["./PlayerQueue-29876489.js", "./ListviewItem-b7a4258b.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-349a0ac0.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-5f240a62.js", "./VDialog-28e4e64e.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./ListviewItem-9fa6da34.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VTabs-13127e50.js", "./VTabs-3cd3e980.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+            component: () => pe(() => import("./PlayerQueue-7ca94b07.js"), ["./PlayerQueue-7ca94b07.js", "./ListviewItem-2bd74fad.js", "./MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-282a676b.js", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VDialog-93a2100b.js", "./VDialog-28e4e64e.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./MediaItemThumb-24a77af5.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./ListviewItem-732a7603.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VTabs-21d8affa.js", "./VTabs-3cd3e980.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
             props: !0
         }, {
             path: "/settings",
             name: "settings",
-            component: () => pe(() => import("./Settings-244fcb0f.js"), ["./Settings-244fcb0f.js", "./VTabs-13127e50.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-336c24cd.js", "./VDivider-bc1524a3.css", "./VTabs-3cd3e980.css"], import.meta.url),
+            component: () => pe(() => import("./Settings-f159e60c.js"), ["./Settings-f159e60c.js", "./VTabs-21d8affa.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VTabs-3cd3e980.css"], import.meta.url),
             props: !0,
             children: [{
                 path: "providers",
                 name: "providersettings",
-                component: () => pe(() => import("./Providers-a361876b.js"), ["./Providers-a361876b.js", "./Container-349a0ac0.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-59559304.js", "./Button-15e2fa72.css", "./Alert-55091fd0.js", "./Alert-c80b13d7.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./Providers-0e527c0c.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
+                component: () => pe(() => import("./Providers-65d3d824.js"), ["./Providers-65d3d824.js", "./Container-282a676b.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-4a781169.js", "./Button-15e2fa72.css", "./Alert-4d78da02.js", "./Alert-c80b13d7.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./Providers-0e527c0c.css", "./vue-virtual-scroller-4d71315f.css"], import.meta.url),
                 props: !0
             }, {
                 path: "players",
                 name: "playersettings",
-                component: () => pe(() => import("./Players-b1f01106.js"), ["./Players-b1f01106.js", "./Container-349a0ac0.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-59559304.js", "./Button-15e2fa72.css"], import.meta.url),
+                component: () => pe(() => import("./Players-5c99fe5e.js"), ["./Players-5c99fe5e.js", "./Container-282a676b.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./Button-4a781169.js", "./Button-15e2fa72.css"], import.meta.url),
                 props: !0
             }, {
                 path: "core",
                 name: "coresettings",
-                component: () => pe(() => import("./CoreConfigs-0b98268a.js"), ["./CoreConfigs-0b98268a.js", "./Container-349a0ac0.js", "./VMenu-bc0cce60.js", "./VDivider-336c24cd.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VToolbar-daf2b89f.js", "./VToolbar-222d6375.css", "./VCard-138864fc.js", "./VCard-103d8462.css"], import.meta.url),
+                component: () => pe(() => import("./CoreConfigs-69940384.js"), ["./CoreConfigs-69940384.js", "./Container-282a676b.js", "./VMenu-ccc026f2.js", "./VDivider-adefbf87.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-bc1524a3.css", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-b930657a.css", "./Container-ed1c67df.css", "./VGrid-b9c72806.css", "./VToolbar-806969a3.js", "./VToolbar-222d6375.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./CoreConfigs-1c0e2549.css"], import.meta.url),
                 props: !0
             }, {
                 path: "addprovider/:domain",
                 name: "addprovider",
-                component: () => pe(() => import("./AddProvider-32056ca3.js"), ["./AddProvider-32056ca3.js", "./index.browser-7e542916.js", "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js", "./VExpansionPanel-67038b00.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-336c24cd.js", "./VDivider-bc1524a3.css", "./VDialog-5f240a62.js", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-bc0cce60.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./VSpacer-bdf2f653.js", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
+                component: () => pe(() => import("./AddProvider-a95ca786.js"), ["./AddProvider-a95ca786.js", "./index.browser-7e542916.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editprovider/:instanceId",
                 name: "editprovider",
-                component: () => pe(() => import("./EditProvider-019f1e2b.js"), ["./EditProvider-019f1e2b.js", "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js", "./VExpansionPanel-67038b00.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-336c24cd.js", "./VDivider-bc1524a3.css", "./VDialog-5f240a62.js", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-bc0cce60.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./VSpacer-bdf2f653.js", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
+                component: () => pe(() => import("./EditProvider-a2553a06.js"), ["./EditProvider-a2553a06.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
                 props: !0
             }, {
                 path: "editplayer/:playerId",
                 name: "editplayer",
-                component: () => pe(() => import("./EditPlayer-19592b08.js"), ["./EditPlayer-19592b08.js", "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js", "./VExpansionPanel-67038b00.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-336c24cd.js", "./VDivider-bc1524a3.css", "./VDialog-5f240a62.js", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-bc0cce60.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./VSpacer-bdf2f653.js", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
+                component: () => pe(() => import("./EditPlayer-f0c55a15.js"), ["./EditPlayer-f0c55a15.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css"], import.meta.url),
                 props: !0
             }, {
                 path: "editcore/:domain",
                 name: "editcore",
-                component: () => pe(() => import("./EditCoreConfig-d3e464b0.js"), ["./EditCoreConfig-d3e464b0.js", "./EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js", "./VExpansionPanel-67038b00.js", "./VBtn-68784d55.js", "./VBtn-76f512af.css", "./VDivider-336c24cd.js", "./VDivider-bc1524a3.css", "./VDialog-5f240a62.js", "./VListItem-230d1393.js", "./VListItem-b9e24cb0.css", "./VMenu-bc0cce60.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-138864fc.js", "./VCard-103d8462.css", "./VSpacer-bdf2f653.js", "./VSelect-04a129eb.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
+                component: () => pe(() => import("./EditCoreConfig-714d074a.js"), ["./EditCoreConfig-714d074a.js", "./EditConfig.vue_vue_type_style_index_0_lang-9825e058.js", "./VExpansionPanel-75456689.js", "./VBtn-61e39030.js", "./VBtn-76f512af.css", "./VDivider-adefbf87.js", "./VDivider-bc1524a3.css", "./VDialog-93a2100b.js", "./VListItem-f848c028.js", "./VListItem-b9e24cb0.css", "./VMenu-ccc026f2.js", "./VMenu-b930657a.css", "./VDialog-28e4e64e.css", "./VExpansionPanel-16e67e58.css", "./VCard-f3e11b51.js", "./VCard-103d8462.css", "./VSpacer-159b0383.js", "./VSelect-a66ffc02.js", "./VSelect-45a454b3.css", "./EditConfig-25e44c20.css", "./index.browser-7e542916.js"], import.meta.url),
                 props: !0
             }, {
                 path: "",
                 redirect: "/settings/providers",
                 name: "settingsredirect"
             }]
         }]
@@ -10607,51 +10597,51 @@
     })))
 });
 /*!
  * shared v9.2.2
  * (c) 2022 kazuya kawaguchi
  * Released under the MIT License.
  */
-const li = typeof window < "u",
+const si = typeof window < "u",
     Mh = typeof Symbol == "function" && typeof Symbol.toStringTag == "symbol",
     Ht = e => Mh ? Symbol(e) : e,
     wh = (e, t, n) => Ch({
         l: e,
         k: t,
         s: n
     }),
     Ch = e => JSON.stringify(e).replace(/\u2028/g, "\\u2028").replace(/\u2029/g, "\\u2029").replace(/\u0027/g, "\\u0027"),
     Ce = e => typeof e == "number" && isFinite(e),
-    kh = e => ta(e) === "[object Date]",
-    Kr = e => ta(e) === "[object RegExp]",
-    bo = e => ae(e) && Object.keys(e).length === 0;
+    kh = e => ea(e) === "[object Date]",
+    qr = e => ea(e) === "[object RegExp]",
+    zo = e => ae(e) && Object.keys(e).length === 0;
 
 function Dh(e, t) {
     typeof console < "u" && (console.warn("[intlify] " + e), t && console.warn(t.stack))
 }
 const Fe = Object.assign;
-let Hs;
-const Ji = () => Hs || (Hs = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
+let Ns;
+const Zi = () => Ns || (Ns = typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : typeof global < "u" ? global : {});
 
-function xs(e) {
+function Hs(e) {
     return e.replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&apos;")
 }
 const Ih = Object.prototype.hasOwnProperty;
 
-function ea(e, t) {
+function Ji(e, t) {
     return Ih.call(e, t)
 }
 const Te = Array.isArray,
     Ie = e => typeof e == "function",
     U = e => typeof e == "string",
     ge = e => typeof e == "boolean",
     ue = e => e !== null && typeof e == "object",
     pu = Object.prototype.toString,
-    ta = e => pu.call(e),
-    ae = e => ta(e) === "[object Object]",
+    ea = e => pu.call(e),
+    ae = e => ea(e) === "[object Object]",
     Oh = e => e == null ? "" : Te(e) || ae(e) && e.toString === pu ? JSON.stringify(e, null, 2) : String(e);
 /*!
  * message-compiler v9.2.2
  * (c) 2022 kazuya kawaguchi
  * Released under the MIT License.
  */
 const hu = {
@@ -10807,24 +10797,24 @@
     }
     for (; r !== null;)
         if (n++, a = e[n], !(a === "\\" && _())) {
             if (c = Bh(a), m = xt[r], l = m[c] || m.l || 8, l === 8 || (r = l[0], l[1] !== void 0 && (d = f[l[1]], d && (u = a, d() === !1)))) return;
             if (r === 7) return t
         }
 }
-const Fs = new Map;
+const xs = new Map;
 
 function xh(e, t) {
     return ue(e) ? e[t] : null
 }
 
 function Fh(e, t) {
     if (!ue(e)) return null;
-    let n = Fs.get(t);
-    if (n || (n = Hh(t), n && Fs.set(t, n)), !n) return null;
+    let n = xs.get(t);
+    if (n || (n = Hh(t), n && xs.set(t, n)), !n) return null;
     const r = n.length;
     let o = e,
         a = 0;
     for (; a < r;) {
         const s = o[n[a]];
         if (s === void 0) return null;
         o = s, a++
@@ -10833,15 +10823,15 @@
 }
 const Vh = e => e,
     Uh = e => "",
     Wh = "text",
     jh = e => e.length === 0 ? "" : e.join(""),
     qh = Oh;
 
-function Vs(e, t) {
+function Fs(e, t) {
     return e = Math.abs(e), t === 2 ? e ? e > 1 ? 1 : 0 : 1 : e ? Math.min(e, 2) : 0
 }
 
 function Kh(e) {
     const t = Ce(e.pluralIndex) ? e.pluralIndex : -1;
     return e.named && (Ce(e.named.count) || Ce(e.named.n)) ? Ce(e.named.count) ? e.named.count : Ce(e.named.n) ? e.named.n : t : t
 }
@@ -10849,16 +10839,16 @@
 function Xh(e, t) {
     t.count || (t.count = e), t.n || (t.n = e)
 }
 
 function $h(e = {}) {
     const t = e.locale,
         n = Kh(e),
-        r = ue(e.pluralRules) && U(t) && Ie(e.pluralRules[t]) ? e.pluralRules[t] : Vs,
-        o = ue(e.pluralRules) && U(t) && Ie(e.pluralRules[t]) ? Vs : void 0,
+        r = ue(e.pluralRules) && U(t) && Ie(e.pluralRules[t]) ? e.pluralRules[t] : Fs,
+        o = ue(e.pluralRules) && U(t) && Ie(e.pluralRules[t]) ? Fs : void 0,
         a = v => v[r(n, v.length, o)],
         s = e.list || [],
         u = v => s[v],
         c = e.named || {};
     Ce(e.pluralIndex) && Xh(n, c);
     const l = v => c[v];
 
@@ -10885,54 +10875,54 @@
             message: d,
             type: p,
             interpolate: _,
             normalize: f
         };
     return T
 }
-let cr = null;
+let lr = null;
 
 function Yh(e) {
-    cr = e
+    lr = e
 }
 
 function Qh(e, t, n) {
-    cr && cr.emit(bu.I18nInit, {
+    lr && lr.emit(bu.I18nInit, {
         timestamp: Date.now(),
         i18n: e,
         version: t,
         meta: n
     })
 }
 const Zh = Jh(bu.FunctionTranslate);
 
 function Jh(e) {
-    return t => cr && cr.emit(e, t)
+    return t => lr && lr.emit(e, t)
 }
 
 function ez(e, t, n) {
     return [...new Set([n, ...Te(t) ? t : ue(t) ? Object.keys(t) : U(t) ? [t] : [n]])]
 }
 
 function gu(e, t, n) {
-    const r = U(n) ? n : na,
+    const r = U(n) ? n : ta,
         o = e;
     o.__localeChainCache || (o.__localeChainCache = new Map);
     let a = o.__localeChainCache.get(r);
     if (!a) {
         a = [];
         let s = [n];
-        for (; Te(s);) s = Us(a, s, t);
+        for (; Te(s);) s = Vs(a, s, t);
         const u = Te(t) || !ae(t) ? t : t.default ? t.default : null;
-        s = U(u) ? [u] : u, Te(s) && Us(a, s, !1), o.__localeChainCache.set(r, a)
+        s = U(u) ? [u] : u, Te(s) && Vs(a, s, !1), o.__localeChainCache.set(r, a)
     }
     return a
 }
 
-function Us(e, t, n) {
+function Vs(e, t, n) {
     let r = !0;
     for (let o = 0; o < t.length && ge(r); o++) {
         const a = t[o];
         U(a) && (r = tz(e, t[o], n))
     }
     return r
 }
@@ -10953,66 +10943,66 @@
         r = t[t.length - 1] !== "!";
         const o = t.replace(/!/g, "");
         e.push(o), (Te(n) || ae(n)) && n[o] && (r = n[o])
     }
     return r
 }
 const rz = "9.2.2",
-    go = -1,
-    na = "en-US",
-    Ws = "",
-    js = e => `${e.charAt(0).toLocaleUpperCase()}${e.substr(1)}`;
+    bo = -1,
+    ta = "en-US",
+    Us = "",
+    Ws = e => `${e.charAt(0).toLocaleUpperCase()}${e.substr(1)}`;
 
 function oz() {
     return {
         upper: (e, t) => t === "text" && U(e) ? e.toUpperCase() : t === "vnode" && ue(e) && "__v_isVNode" in e ? e.children.toUpperCase() : e,
         lower: (e, t) => t === "text" && U(e) ? e.toLowerCase() : t === "vnode" && ue(e) && "__v_isVNode" in e ? e.children.toLowerCase() : e,
-        capitalize: (e, t) => t === "text" && U(e) ? js(e) : t === "vnode" && ue(e) && "__v_isVNode" in e ? js(e.children) : e
+        capitalize: (e, t) => t === "text" && U(e) ? Ws(e) : t === "vnode" && ue(e) && "__v_isVNode" in e ? Ws(e.children) : e
     }
 }
 let iz, yu;
 
 function az(e) {
     yu = e
 }
 let vu;
 
 function sz(e) {
     vu = e
 }
 let Tu = null;
-const qs = e => {
+const js = e => {
         Tu = e
     },
     lz = () => Tu;
 let Su = null;
-const Ks = e => {
+const qs = e => {
         Su = e
     },
     cz = () => Su;
-let Xs = 0;
+let Ks = 0;
 
 function uz(e = {}) {
     const t = U(e.version) ? e.version : rz,
-        n = U(e.locale) ? e.locale : na,
+        n = U(e.locale) ? e.locale : ta,
         r = Te(e.fallbackLocale) || ae(e.fallbackLocale) || U(e.fallbackLocale) || e.fallbackLocale === !1 ? e.fallbackLocale : n,
         o = ae(e.messages) ? e.messages : {
             [n]: {}
         },
         a = ae(e.datetimeFormats) ? e.datetimeFormats : {
             [n]: {}
         },
         s = ae(e.numberFormats) ? e.numberFormats : {
             [n]: {}
         },
         u = Fe({}, e.modifiers || {}, oz()),
         c = e.pluralRules || {},
         l = Ie(e.missing) ? e.missing : null,
-        d = ge(e.missingWarn) || Kr(e.missingWarn) ? e.missingWarn : !0,
-        m = ge(e.fallbackWarn) || Kr(e.fallbackWarn) ? e.fallbackWarn : !0,
+        d = ge(e.missingWarn) || qr(e.missingWarn) ? e.missingWarn : !0,
+        m = ge(e.fallbackWarn) || qr(e.fallbackWarn) ? e.fallbackWarn : !0,
         f = !!e.fallbackFormat,
         _ = !!e.unresolving,
         p = Ie(e.postTranslation) ? e.postTranslation : null,
         b = ae(e.processor) ? e.processor : null,
         T = ge(e.warnHtmlMessage) ? e.warnHtmlMessage : !0,
         v = !!e.escapeParameter,
         A = Ie(e.messageCompiler) ? e.messageCompiler : iz,
@@ -11020,18 +11010,18 @@
         P = Ie(e.localeFallbacker) ? e.localeFallbacker : vu || ez,
         M = ue(e.fallbackContext) ? e.fallbackContext : void 0,
         N = Ie(e.onWarn) ? e.onWarn : Dh,
         j = e,
         L = ue(j.__datetimeFormatters) ? j.__datetimeFormatters : new Map,
         X = ue(j.__numberFormatters) ? j.__numberFormatters : new Map,
         $ = ue(j.__meta) ? j.__meta : {};
-    Xs++;
+    Ks++;
     const Y = {
         version: t,
-        cid: Xs,
+        cid: Ks,
         locale: n,
         fallbackLocale: r,
         messages: o,
         modifiers: u,
         pluralRules: c,
         missing: l,
         missingWarn: d,
@@ -11048,56 +11038,56 @@
         fallbackContext: M,
         onWarn: N,
         __meta: $
     };
     return Y.datetimeFormats = a, Y.numberFormats = s, Y.__datetimeFormatters = L, Y.__numberFormatters = X, __INTLIFY_PROD_DEVTOOLS__ && Qh(Y, t, $), Y
 }
 
-function ra(e, t, n, r, o) {
+function na(e, t, n, r, o) {
     const {
         missing: a,
         onWarn: s
     } = e;
     if (a !== null) {
         const u = a(e, n, t, o);
         return U(u) ? u : t
     } else return t
 }
 
-function Hn(e, t, n) {
+function Nn(e, t, n) {
     const r = e;
     r.__localeChainCache = new Map, e.localeFallbacker(e, n, t)
 }
 let Au = hu.__EXTEND_POINT__;
-const Lo = () => ++Au,
-    gn = {
+const Ro = () => ++Au,
+    bn = {
         INVALID_ARGUMENT: Au,
-        INVALID_DATE_ARGUMENT: Lo(),
-        INVALID_ISO_DATE_ARGUMENT: Lo(),
-        __EXTEND_POINT__: Lo()
+        INVALID_DATE_ARGUMENT: Ro(),
+        INVALID_ISO_DATE_ARGUMENT: Ro(),
+        __EXTEND_POINT__: Ro()
     };
 
-function yn(e) {
+function gn(e) {
     return zu(e, null, void 0)
 }
-const $s = () => "",
+const Xs = () => "",
     zt = e => Ie(e);
 
-function Ys(e, ...t) {
+function $s(e, ...t) {
     const {
         fallbackFormat: n,
         postTranslation: r,
         unresolving: o,
         messageCompiler: a,
         fallbackLocale: s,
         messages: u
-    } = e, [c, l] = ci(...t), d = ge(l.missingWarn) ? l.missingWarn : e.missingWarn, m = ge(l.fallbackWarn) ? l.fallbackWarn : e.fallbackWarn, f = ge(l.escapeParameter) ? l.escapeParameter : e.escapeParameter, _ = !!l.resolvedMessage, p = U(l.default) || ge(l.default) ? ge(l.default) ? a ? c : () => c : l.default : n ? a ? c : () => c : "", b = n || p !== "", T = U(l.locale) ? l.locale : e.locale;
+    } = e, [c, l] = li(...t), d = ge(l.missingWarn) ? l.missingWarn : e.missingWarn, m = ge(l.fallbackWarn) ? l.fallbackWarn : e.fallbackWarn, f = ge(l.escapeParameter) ? l.escapeParameter : e.escapeParameter, _ = !!l.resolvedMessage, p = U(l.default) || ge(l.default) ? ge(l.default) ? a ? c : () => c : l.default : n ? a ? c : () => c : "", b = n || p !== "", T = U(l.locale) ? l.locale : e.locale;
     f && mz(l);
     let [v, A, I] = _ ? [c, T, u[T] || {}] : Pu(e, c, T, s, m, d), P = v, M = c;
-    if (!_ && !(U(P) || zt(P)) && b && (P = p, M = P), !_ && (!(U(P) || zt(P)) || !U(A))) return o ? go : c;
+    if (!_ && !(U(P) || zt(P)) && b && (P = p, M = P), !_ && (!(U(P) || zt(P)) || !U(A))) return o ? bo : c;
     let N = !1;
     const j = () => {
             N = !0
         },
         L = zt(P) ? P : Eu(e, c, A, P, M, j);
     if (N) return P;
     const X = _z(e, A, I, l),
@@ -11114,31 +11104,31 @@
         };
         te.meta = Fe({}, e.__meta, lz() || {}), Zh(te)
     }
     return x
 }
 
 function mz(e) {
-    Te(e.list) ? e.list = e.list.map(t => U(t) ? xs(t) : t) : ue(e.named) && Object.keys(e.named).forEach(t => {
-        U(e.named[t]) && (e.named[t] = xs(e.named[t]))
+    Te(e.list) ? e.list = e.list.map(t => U(t) ? Hs(t) : t) : ue(e.named) && Object.keys(e.named).forEach(t => {
+        U(e.named[t]) && (e.named[t] = Hs(e.named[t]))
     })
 }
 
 function Pu(e, t, n, r, o, a) {
     const {
         messages: s,
         onWarn: u,
         messageResolver: c,
         localeFallbacker: l
     } = e, d = l(e, r, n);
     let m = {},
         f, _ = null;
     const p = "translate";
     for (let b = 0; b < d.length && (f = d[b], m = s[f] || {}, (_ = c(m, t)) === null && (_ = m[t]), !(U(_) || Ie(_))); b++) {
-        const T = ra(e, t, f, a, p);
+        const T = na(e, t, f, a, p);
         T !== t && (_ = T)
     }
     return [_, f, m]
 }
 
 function Eu(e, t, n, r, o, a) {
     const {
@@ -11157,19 +11147,19 @@
     return c.locale = n, c.key = t, c.source = r, c
 }
 
 function dz(e, t, n) {
     return t(n)
 }
 
-function ci(...e) {
+function li(...e) {
     const [t, n, r] = e, o = {};
-    if (!U(t) && !Ce(t) && !zt(t)) throw yn(gn.INVALID_ARGUMENT);
+    if (!U(t) && !Ce(t) && !zt(t)) throw gn(bn.INVALID_ARGUMENT);
     const a = Ce(t) ? String(t) : (zt(t), t);
-    return Ce(n) ? o.plural = n : U(n) ? o.default = n : ae(n) && !bo(n) ? o.named = n : Te(n) && (o.list = n), Ce(r) ? o.plural = r : U(r) ? o.default = r : ae(r) && Fe(o, r), [a, o]
+    return Ce(n) ? o.plural = n : U(n) ? o.default = n : ae(n) && !zo(n) ? o.named = n : Te(n) && (o.list = n), Ce(r) ? o.plural = r : U(r) ? o.default = r : ae(r) && Fe(o, r), [a, o]
 }
 
 function fz(e, t, n, r, o, a) {
     return {
         warnHtmlMessage: o,
         onError: s => {
             throw a && a(s), s
@@ -11198,134 +11188,134 @@
                 p = s(b, _)
             }
             if (U(p)) {
                 let b = !1;
                 const v = Eu(e, _, t, p, _, () => {
                     b = !0
                 });
-                return b ? $s : v
-            } else return zt(p) ? p : $s
+                return b ? Xs : v
+            } else return zt(p) ? p : Xs
         }
     };
     return e.processor && (f.processor = e.processor), r.list && (f.list = r.list), r.named && (f.named = r.named), Ce(r.plural) && (f.pluralIndex = r.plural), f
 }
 
-function Qs(e, ...t) {
+function Ys(e, ...t) {
     const {
         datetimeFormats: n,
         unresolving: r,
         fallbackLocale: o,
         onWarn: a,
         localeFallbacker: s
     } = e, {
         __datetimeFormatters: u
-    } = e, [c, l, d, m] = ui(...t), f = ge(d.missingWarn) ? d.missingWarn : e.missingWarn;
+    } = e, [c, l, d, m] = ci(...t), f = ge(d.missingWarn) ? d.missingWarn : e.missingWarn;
     ge(d.fallbackWarn) ? d.fallbackWarn : e.fallbackWarn;
     const _ = !!d.part,
         p = U(d.locale) ? d.locale : e.locale,
         b = s(e, o, p);
     if (!U(c) || c === "") return new Intl.DateTimeFormat(p, m).format(l);
     let T = {},
         v, A = null;
     const I = "datetime format";
-    for (let N = 0; N < b.length && (v = b[N], T = n[v] || {}, A = T[c], !ae(A)); N++) ra(e, c, v, f, I);
-    if (!ae(A) || !U(v)) return r ? go : c;
+    for (let N = 0; N < b.length && (v = b[N], T = n[v] || {}, A = T[c], !ae(A)); N++) na(e, c, v, f, I);
+    if (!ae(A) || !U(v)) return r ? bo : c;
     let P = `${v}__${c}`;
-    bo(m) || (P = `${P}__${JSON.stringify(m)}`);
+    zo(m) || (P = `${P}__${JSON.stringify(m)}`);
     let M = u.get(P);
     return M || (M = new Intl.DateTimeFormat(v, Fe({}, A, m)), u.set(P, M)), _ ? M.formatToParts(l) : M.format(l)
 }
 const Mu = ["localeMatcher", "weekday", "era", "year", "month", "day", "hour", "minute", "second", "timeZoneName", "formatMatcher", "hour12", "timeZone", "dateStyle", "timeStyle", "calendar", "dayPeriod", "numberingSystem", "hourCycle", "fractionalSecondDigits"];
 
-function ui(...e) {
+function ci(...e) {
     const [t, n, r, o] = e, a = {};
     let s = {},
         u;
     if (U(t)) {
         const c = t.match(/(\d{4}-\d{2}-\d{2})(T|\s)?(.*)/);
-        if (!c) throw yn(gn.INVALID_ISO_DATE_ARGUMENT);
+        if (!c) throw gn(bn.INVALID_ISO_DATE_ARGUMENT);
         const l = c[3] ? c[3].trim().startsWith("T") ? `${c[1].trim()}${c[3].trim()}` : `${c[1].trim()}T${c[3].trim()}` : c[1].trim();
         u = new Date(l);
         try {
             u.toISOString()
         } catch {
-            throw yn(gn.INVALID_ISO_DATE_ARGUMENT)
+            throw gn(bn.INVALID_ISO_DATE_ARGUMENT)
         }
     } else if (kh(t)) {
-        if (isNaN(t.getTime())) throw yn(gn.INVALID_DATE_ARGUMENT);
+        if (isNaN(t.getTime())) throw gn(bn.INVALID_DATE_ARGUMENT);
         u = t
     } else if (Ce(t)) u = t;
-    else throw yn(gn.INVALID_ARGUMENT);
+    else throw gn(bn.INVALID_ARGUMENT);
     return U(n) ? a.key = n : ae(n) && Object.keys(n).forEach(c => {
         Mu.includes(c) ? s[c] = n[c] : a[c] = n[c]
     }), U(r) ? a.locale = r : ae(r) && (s = r), ae(o) && (s = o), [a.key || "", u, a, s]
 }
 
-function Zs(e, t, n) {
+function Qs(e, t, n) {
     const r = e;
     for (const o in n) {
         const a = `${t}__${o}`;
         r.__datetimeFormatters.has(a) && r.__datetimeFormatters.delete(a)
     }
 }
 
-function Js(e, ...t) {
+function Zs(e, ...t) {
     const {
         numberFormats: n,
         unresolving: r,
         fallbackLocale: o,
         onWarn: a,
         localeFallbacker: s
     } = e, {
         __numberFormatters: u
-    } = e, [c, l, d, m] = mi(...t), f = ge(d.missingWarn) ? d.missingWarn : e.missingWarn;
+    } = e, [c, l, d, m] = ui(...t), f = ge(d.missingWarn) ? d.missingWarn : e.missingWarn;
     ge(d.fallbackWarn) ? d.fallbackWarn : e.fallbackWarn;
     const _ = !!d.part,
         p = U(d.locale) ? d.locale : e.locale,
         b = s(e, o, p);
     if (!U(c) || c === "") return new Intl.NumberFormat(p, m).format(l);
     let T = {},
         v, A = null;
     const I = "number format";
-    for (let N = 0; N < b.length && (v = b[N], T = n[v] || {}, A = T[c], !ae(A)); N++) ra(e, c, v, f, I);
-    if (!ae(A) || !U(v)) return r ? go : c;
+    for (let N = 0; N < b.length && (v = b[N], T = n[v] || {}, A = T[c], !ae(A)); N++) na(e, c, v, f, I);
+    if (!ae(A) || !U(v)) return r ? bo : c;
     let P = `${v}__${c}`;
-    bo(m) || (P = `${P}__${JSON.stringify(m)}`);
+    zo(m) || (P = `${P}__${JSON.stringify(m)}`);
     let M = u.get(P);
     return M || (M = new Intl.NumberFormat(v, Fe({}, A, m)), u.set(P, M)), _ ? M.formatToParts(l) : M.format(l)
 }
 const wu = ["localeMatcher", "style", "currency", "currencyDisplay", "currencySign", "useGrouping", "minimumIntegerDigits", "minimumFractionDigits", "maximumFractionDigits", "minimumSignificantDigits", "maximumSignificantDigits", "compactDisplay", "notation", "signDisplay", "unit", "unitDisplay", "roundingMode", "roundingPriority", "roundingIncrement", "trailingZeroDisplay"];
 
-function mi(...e) {
+function ui(...e) {
     const [t, n, r, o] = e, a = {};
     let s = {};
-    if (!Ce(t)) throw yn(gn.INVALID_ARGUMENT);
+    if (!Ce(t)) throw gn(bn.INVALID_ARGUMENT);
     const u = t;
     return U(n) ? a.key = n : ae(n) && Object.keys(n).forEach(c => {
         wu.includes(c) ? s[c] = n[c] : a[c] = n[c]
     }), U(r) ? a.locale = r : ae(r) && (s = r), ae(o) && (s = o), [a.key || "", u, a, s]
 }
 
-function el(e, t, n) {
+function Js(e, t, n) {
     const r = e;
     for (const o in n) {
         const a = `${t}__${o}`;
         r.__numberFormatters.has(a) && r.__numberFormatters.delete(a)
     }
 }
-typeof __INTLIFY_PROD_DEVTOOLS__ != "boolean" && (Ji().__INTLIFY_PROD_DEVTOOLS__ = !1);
+typeof __INTLIFY_PROD_DEVTOOLS__ != "boolean" && (Zi().__INTLIFY_PROD_DEVTOOLS__ = !1);
 /*!
  * vue-i18n v9.2.2
  * (c) 2022 kazuya kawaguchi
  * Released under the MIT License.
  */
 const pz = "9.2.2";
 
 function hz() {
-    typeof __INTLIFY_PROD_DEVTOOLS__ != "boolean" && (Ji().__INTLIFY_PROD_DEVTOOLS__ = !1)
+    typeof __INTLIFY_PROD_DEVTOOLS__ != "boolean" && (Zi().__INTLIFY_PROD_DEVTOOLS__ = !1)
 }
 let Cu = hu.__EXTEND_POINT__;
 const Ve = () => ++Cu,
     Ye = {
         UNEXPECTED_RETURN_TYPE: Cu,
         INVALID_ARGUMENT: Ve(),
         MUST_BE_CALL_SETUP_TOP: Ve(),
@@ -11342,32 +11332,32 @@
         NOT_AVAILABLE_COMPOSITION_IN_LEGACY: Ve(),
         __EXTEND_POINT__: Ve()
     };
 
 function rt(e, ...t) {
     return zu(e, null, void 0)
 }
-const di = Ht("__transrateVNode"),
-    fi = Ht("__datetimeParts"),
-    _i = Ht("__numberParts"),
+const mi = Ht("__transrateVNode"),
+    di = Ht("__datetimeParts"),
+    fi = Ht("__numberParts"),
     zz = Ht("__setPluralRules");
 Ht("__intlifyMeta");
 const bz = Ht("__injectWithOption");
 
-function pi(e) {
+function _i(e) {
     if (!ue(e)) return e;
     for (const t in e)
-        if (ea(e, t))
-            if (!t.includes(".")) ue(e[t]) && pi(e[t]);
+        if (Ji(e, t))
+            if (!t.includes(".")) ue(e[t]) && _i(e[t]);
             else {
                 const n = t.split("."),
                     r = n.length - 1;
                 let o = e;
                 for (let a = 0; a < r; a++) n[a] in o || (o[n[a]] = {}), o = o[n[a]];
-                o[n[r]] = e[t], delete e[t], ue(o[n[r]]) && pi(o[n[r]])
+                o[n[r]] = e[t], delete e[t], ue(o[n[r]]) && _i(o[n[r]])
             } return e
 }
 
 function ku(e, t) {
     const {
         messages: n,
         __i18n: r,
@@ -11378,25 +11368,25 @@
     };
     if (Te(r) && r.forEach(u => {
             if ("locale" in u && "resource" in u) {
                 const {
                     locale: c,
                     resource: l
                 } = u;
-                c ? (s[c] = s[c] || {}, $n(l, s[c])) : $n(l, s)
-            } else U(u) && $n(JSON.parse(u), s)
+                c ? (s[c] = s[c] || {}, Xn(l, s[c])) : Xn(l, s)
+            } else U(u) && Xn(JSON.parse(u), s)
         }), o == null && a)
-        for (const u in s) ea(s, u) && pi(s[u]);
+        for (const u in s) Ji(s, u) && _i(s[u]);
     return s
 }
-const Cr = e => !ue(e) || Te(e);
+const wr = e => !ue(e) || Te(e);
 
-function $n(e, t) {
-    if (Cr(e) || Cr(t)) throw rt(Ye.INVALID_VALUE);
-    for (const n in e) ea(e, n) && (Cr(e[n]) || Cr(t[n]) ? t[n] = e[n] : $n(e[n], t[n]))
+function Xn(e, t) {
+    if (wr(e) || wr(t)) throw rt(Ye.INVALID_VALUE);
+    for (const n in e) Ji(e, n) && (wr(e[n]) || wr(t[n]) ? t[n] = e[n] : Xn(e[n], t[n]))
 }
 
 function Du(e) {
     return e.type
 }
 
 function gz(e, t, n) {
@@ -11420,59 +11410,59 @@
             a.length && a.forEach(s => {
                 e.mergeNumberFormat(s, t.numberFormats[s])
             })
         }
     }
 }
 
-function tl(e) {
-    return fe(mr, null, e, 0)
+function el(e) {
+    return fe(ur, null, e, 0)
 }
-const nl = "__INTLIFY_META__";
-let rl = 0;
+const tl = "__INTLIFY_META__";
+let nl = 0;
 
-function ol(e) {
-    return (t, n, r, o) => e(n, r, On() || void 0, o)
+function rl(e) {
+    return (t, n, r, o) => e(n, r, In() || void 0, o)
 }
 const yz = () => {
-    const e = On();
+    const e = In();
     let t = null;
-    return e && (t = Du(e)[nl]) ? {
-        [nl]: t
+    return e && (t = Du(e)[tl]) ? {
+        [tl]: t
     } : null
 };
 
 function Iu(e = {}, t) {
     const {
         __root: n
     } = e, r = n === void 0;
     let o = ge(e.inheritLocale) ? e.inheritLocale : !0;
-    const a = Me(n && o ? n.locale.value : U(e.locale) ? e.locale : na),
+    const a = Me(n && o ? n.locale.value : U(e.locale) ? e.locale : ta),
         s = Me(n && o ? n.fallbackLocale.value : U(e.fallbackLocale) || Te(e.fallbackLocale) || ae(e.fallbackLocale) || e.fallbackLocale === !1 ? e.fallbackLocale : a.value),
         u = Me(ku(a.value, e)),
         c = Me(ae(e.datetimeFormats) ? e.datetimeFormats : {
             [a.value]: {}
         }),
         l = Me(ae(e.numberFormats) ? e.numberFormats : {
             [a.value]: {}
         });
-    let d = n ? n.missingWarn : ge(e.missingWarn) || Kr(e.missingWarn) ? e.missingWarn : !0,
-        m = n ? n.fallbackWarn : ge(e.fallbackWarn) || Kr(e.fallbackWarn) ? e.fallbackWarn : !0,
+    let d = n ? n.missingWarn : ge(e.missingWarn) || qr(e.missingWarn) ? e.missingWarn : !0,
+        m = n ? n.fallbackWarn : ge(e.fallbackWarn) || qr(e.fallbackWarn) ? e.fallbackWarn : !0,
         f = n ? n.fallbackRoot : ge(e.fallbackRoot) ? e.fallbackRoot : !0,
         _ = !!e.fallbackFormat,
         p = Ie(e.missing) ? e.missing : null,
-        b = Ie(e.missing) ? ol(e.missing) : null,
+        b = Ie(e.missing) ? rl(e.missing) : null,
         T = Ie(e.postTranslation) ? e.postTranslation : null,
         v = n ? n.warnHtmlMessage : ge(e.warnHtmlMessage) ? e.warnHtmlMessage : !0,
         A = !!e.escapeParameter;
     const I = n ? n.modifiers : ae(e.modifiers) ? e.modifiers : {};
     let P = e.pluralRules || n && n.pluralRules,
         M;
     M = (() => {
-        r && Ks(null);
+        r && qs(null);
         const y = {
             version: pz,
             locale: a.value,
             fallbackLocale: s.value,
             messages: u.value,
             modifiers: I,
             pluralRules: P,
@@ -11487,30 +11477,30 @@
             messageResolver: e.messageResolver,
             __meta: {
                 framework: "vue"
             }
         };
         y.datetimeFormats = c.value, y.numberFormats = l.value, y.__datetimeFormatters = ae(M) ? M.__datetimeFormatters : void 0, y.__numberFormatters = ae(M) ? M.__numberFormatters : void 0;
         const S = uz(y);
-        return r && Ks(S), S
-    })(), Hn(M, a.value, s.value);
+        return r && qs(S), S
+    })(), Nn(M, a.value, s.value);
 
     function j() {
         return [a.value, s.value, u.value, c.value, l.value]
     }
     const L = re({
             get: () => a.value,
             set: y => {
                 a.value = y, M.locale = a.value
             }
         }),
         X = re({
             get: () => s.value,
             set: y => {
-                s.value = y, M.fallbackLocale = s.value, Hn(M, a.value, y)
+                s.value = y, M.fallbackLocale = s.value, Nn(M, a.value, y)
             }
         }),
         $ = re(() => u.value),
         Y = re(() => c.value),
         x = re(() => l.value);
 
     function te() {
@@ -11522,81 +11512,81 @@
     }
 
     function ot() {
         return p
     }
 
     function _e(y) {
-        y !== null && (b = ol(y)), p = y, M.missing = b
+        y !== null && (b = rl(y)), p = y, M.missing = b
     }
     const ne = (y, S, F, W, Z, le) => {
         j();
         let J;
         if (__INTLIFY_PROD_DEVTOOLS__) try {
-            qs(yz()), r || (M.fallbackContext = n ? cz() : void 0), J = y(M)
+            js(yz()), r || (M.fallbackContext = n ? cz() : void 0), J = y(M)
         } finally {
-            qs(null), r || (M.fallbackContext = void 0)
+            js(null), r || (M.fallbackContext = void 0)
         } else J = y(M);
-        if (Ce(J) && J === go) {
+        if (Ce(J) && J === bo) {
             const [he, Ze] = S();
             return n && f ? W(n) : Z(he)
         } else {
             if (le(J)) return J;
             throw rt(Ye.UNEXPECTED_RETURN_TYPE)
         }
     };
 
     function oe(...y) {
-        return ne(S => Reflect.apply(Ys, null, [S, ...y]), () => ci(...y), "translate", S => Reflect.apply(S.t, S, [...y]), S => S, S => U(S))
+        return ne(S => Reflect.apply($s, null, [S, ...y]), () => li(...y), "translate", S => Reflect.apply(S.t, S, [...y]), S => S, S => U(S))
     }
 
     function it(...y) {
         const [S, F, W] = y;
         if (W && !ue(W)) throw rt(Ye.INVALID_ARGUMENT);
         return oe(S, F, Fe({
             resolvedMessage: !0
         }, W || {}))
     }
 
     function ft(...y) {
-        return ne(S => Reflect.apply(Qs, null, [S, ...y]), () => ui(...y), "datetime format", S => Reflect.apply(S.d, S, [...y]), () => Ws, S => U(S))
+        return ne(S => Reflect.apply(Ys, null, [S, ...y]), () => ci(...y), "datetime format", S => Reflect.apply(S.d, S, [...y]), () => Us, S => U(S))
     }
 
     function Qe(...y) {
-        return ne(S => Reflect.apply(Js, null, [S, ...y]), () => mi(...y), "number format", S => Reflect.apply(S.n, S, [...y]), () => Ws, S => U(S))
+        return ne(S => Reflect.apply(Zs, null, [S, ...y]), () => ui(...y), "number format", S => Reflect.apply(S.n, S, [...y]), () => Us, S => U(S))
     }
 
     function Ge(y) {
-        return y.map(S => U(S) || Ce(S) || ge(S) ? tl(String(S)) : S)
+        return y.map(S => U(S) || Ce(S) || ge(S) ? el(String(S)) : S)
     }
     const Mt = {
         normalize: Ge,
         interpolate: y => y,
         type: "vnode"
     };
 
     function an(...y) {
         return ne(S => {
             let F;
             const W = S;
             try {
-                W.processor = Mt, F = Reflect.apply(Ys, null, [W, ...y])
+                W.processor = Mt, F = Reflect.apply($s, null, [W, ...y])
             } finally {
                 W.processor = null
             }
             return F
-        }, () => ci(...y), "translate", S => S[di](...y), S => [tl(S)], S => Te(S))
+        }, () => li(...y), "translate", S => S[mi](...y), S => [el(S)], S => Te(S))
     }
 
     function Pe(...y) {
-        return ne(S => Reflect.apply(Js, null, [S, ...y]), () => mi(...y), "number format", S => S[_i](...y), () => [], S => U(S) || Te(S))
+        return ne(S => Reflect.apply(Zs, null, [S, ...y]), () => ui(...y), "number format", S => S[fi](...y), () => [], S => U(S) || Te(S))
     }
 
     function w(...y) {
-        return ne(S => Reflect.apply(Qs, null, [S, ...y]), () => ui(...y), "datetime format", S => S[fi](...y), () => [], S => U(S) || Te(S))
+        return ne(S => Reflect.apply(Ys, null, [S, ...y]), () => ci(...y), "datetime format", S => S[di](...y), () => [], S => U(S) || Te(S))
     }
 
     function H(y) {
         P = y, M.pluralRules = P
     }
 
     function R(y, S) {
@@ -11629,54 +11619,54 @@
     }
 
     function z(y, S) {
         u.value[y] = S, M.messages = u.value
     }
 
     function g(y, S) {
-        u.value[y] = u.value[y] || {}, $n(S, u.value[y]), M.messages = u.value
+        u.value[y] = u.value[y] || {}, Xn(S, u.value[y]), M.messages = u.value
     }
 
     function E(y) {
         return c.value[y] || {}
     }
 
     function k(y, S) {
-        c.value[y] = S, M.datetimeFormats = c.value, Zs(M, y, S)
+        c.value[y] = S, M.datetimeFormats = c.value, Qs(M, y, S)
     }
 
     function D(y, S) {
-        c.value[y] = Fe(c.value[y] || {}, S), M.datetimeFormats = c.value, Zs(M, y, S)
+        c.value[y] = Fe(c.value[y] || {}, S), M.datetimeFormats = c.value, Qs(M, y, S)
     }
 
     function B(y) {
         return l.value[y] || {}
     }
 
     function O(y, S) {
-        l.value[y] = S, M.numberFormats = l.value, el(M, y, S)
+        l.value[y] = S, M.numberFormats = l.value, Js(M, y, S)
     }
 
     function G(y, S) {
-        l.value[y] = Fe(l.value[y] || {}, S), M.numberFormats = l.value, el(M, y, S)
+        l.value[y] = Fe(l.value[y] || {}, S), M.numberFormats = l.value, Js(M, y, S)
     }
-    rl++, n && li && (xe(n.locale, y => {
-        o && (a.value = y, M.locale = y, Hn(M, a.value, s.value))
+    nl++, n && si && (xe(n.locale, y => {
+        o && (a.value = y, M.locale = y, Nn(M, a.value, s.value))
     }), xe(n.fallbackLocale, y => {
-        o && (s.value = y, M.fallbackLocale = y, Hn(M, a.value, s.value))
+        o && (s.value = y, M.fallbackLocale = y, Nn(M, a.value, s.value))
     }));
     const C = {
-        id: rl,
+        id: nl,
         locale: L,
         fallbackLocale: X,
         get inheritLocale() {
             return o
         },
         set inheritLocale(y) {
-            o = y, y && n && (a.value = n.locale.value, s.value = n.fallbackLocale.value, Hn(M, a.value, s.value))
+            o = y, y && n && (a.value = n.locale.value, s.value = n.fallbackLocale.value, Nn(M, a.value, s.value))
         },
         get availableLocales() {
             return Object.keys(u.value).sort()
         },
         messages: $,
         get modifiers() {
             return I
@@ -11729,17 +11719,17 @@
         mergeLocaleMessage: g,
         getPostTranslationHandler: te,
         setPostTranslationHandler: De,
         getMissingHandler: ot,
         setMissingHandler: _e,
         [zz]: H
     };
-    return C.datetimeFormats = Y, C.numberFormats = x, C.rt = it, C.te = R, C.tm = se, C.d = ft, C.n = Qe, C.getDateTimeFormat = E, C.setDateTimeFormat = k, C.mergeDateTimeFormat = D, C.getNumberFormat = B, C.setNumberFormat = O, C.mergeNumberFormat = G, C[bz] = e.__injectWithOption, C[di] = an, C[fi] = w, C[_i] = Pe, C
+    return C.datetimeFormats = Y, C.numberFormats = x, C.rt = it, C.te = R, C.tm = se, C.d = ft, C.n = Qe, C.getDateTimeFormat = E, C.setDateTimeFormat = k, C.mergeDateTimeFormat = D, C.getNumberFormat = B, C.setNumberFormat = O, C.mergeNumberFormat = G, C[bz] = e.__injectWithOption, C[mi] = an, C[di] = w, C[fi] = Pe, C
 }
-const oa = {
+const ra = {
     tag: {
         type: [String, Object]
     },
     locale: {
         type: String
     },
     scope: {
@@ -11760,40 +11750,40 @@
         return o && (n[r] = o()), n
     }, {})
 }
 
 function Ou(e) {
     return He
 }
-const il = {
+const ol = {
     name: "i18n-t",
     props: Fe({
         keypath: {
             type: String,
             required: !0
         },
         plural: {
             type: [Number, String],
             validator: e => Ce(e) || !isNaN(e)
         }
-    }, oa),
+    }, ra),
     setup(e, t) {
         const {
             slots: n,
             attrs: r
-        } = t, o = e.i18n || ia({
+        } = t, o = e.i18n || oa({
             useScope: e.scope,
             __useComponent: !0
         });
         return () => {
             const a = Object.keys(n).filter(m => m !== "_"),
                 s = {};
             e.locale && (s.locale = e.locale), e.plural !== void 0 && (s.plural = U(e.plural) ? +e.plural : e.plural);
             const u = vz(t, a),
-                c = o[di](e.keypath, u, s),
+                c = o[mi](e.keypath, u, s),
                 l = Fe({}, r),
                 d = U(e.tag) || ue(e.tag) ? e.tag : Ou();
             return rn(d, l, c)
         }
     }
 };
 
@@ -11826,50 +11816,50 @@
             return Tz(b) && (b[0].key = `${f.type}-${_}`), b
         }) : U(c) && (l = [c]);
         const d = Fe({}, a),
             m = U(e.tag) || ue(e.tag) ? e.tag : Ou();
         return rn(m, d, l)
     }
 }
-const al = {
+const il = {
         name: "i18n-n",
         props: Fe({
             value: {
                 type: Number,
                 required: !0
             },
             format: {
                 type: [String, Object]
             }
-        }, oa),
+        }, ra),
         setup(e, t) {
-            const n = e.i18n || ia({
+            const n = e.i18n || oa({
                 useScope: "parent",
                 __useComponent: !0
             });
-            return Gu(e, t, wu, (...r) => n[_i](...r))
+            return Gu(e, t, wu, (...r) => n[fi](...r))
         }
     },
-    sl = {
+    al = {
         name: "i18n-d",
         props: Fe({
             value: {
                 type: [Number, Date],
                 required: !0
             },
             format: {
                 type: [String, Object]
             }
-        }, oa),
+        }, ra),
         setup(e, t) {
-            const n = e.i18n || ia({
+            const n = e.i18n || oa({
                 useScope: "parent",
                 __useComponent: !0
             });
-            return Gu(e, t, Mu, (...r) => n[fi](...r))
+            return Gu(e, t, Mu, (...r) => n[di](...r))
         }
     };
 
 function Sz(e, t) {
     const n = e;
     if (e.mode === "composition") return n.__getInstance(t) || e.global; {
         const r = n.__getInstance(t);
@@ -11882,70 +11872,70 @@
         const {
             instance: u,
             modifiers: c,
             value: l
         } = s;
         if (!u || !u.$) throw rt(Ye.UNEXPECTED_ERROR);
         const d = Sz(e, u.$),
-            m = ll(l);
-        return [Reflect.apply(d.t, d, [...cl(m)]), d]
+            m = sl(l);
+        return [Reflect.apply(d.t, d, [...ll(m)]), d]
     };
     return {
         created: (s, u) => {
             const [c, l] = t(u);
-            li && e.global === l && (s.__i18nWatcher = xe(l.locale, () => {
+            si && e.global === l && (s.__i18nWatcher = xe(l.locale, () => {
                 u.instance && u.instance.$forceUpdate()
             })), s.__composer = l, s.textContent = c
         },
         unmounted: s => {
-            li && s.__i18nWatcher && (s.__i18nWatcher(), s.__i18nWatcher = void 0, delete s.__i18nWatcher), s.__composer && (s.__composer = void 0, delete s.__composer)
+            si && s.__i18nWatcher && (s.__i18nWatcher(), s.__i18nWatcher = void 0, delete s.__i18nWatcher), s.__composer && (s.__composer = void 0, delete s.__composer)
         },
         beforeUpdate: (s, {
             value: u
         }) => {
             if (s.__composer) {
                 const c = s.__composer,
-                    l = ll(u);
-                s.textContent = Reflect.apply(c.t, c, [...cl(l)])
+                    l = sl(u);
+                s.textContent = Reflect.apply(c.t, c, [...ll(l)])
             }
         },
         getSSRProps: s => {
             const [u] = t(s);
             return {
                 textContent: u
             }
         }
     }
 }
 
-function ll(e) {
+function sl(e) {
     if (U(e)) return {
         path: e
     };
     if (ae(e)) {
         if (!("path" in e)) throw rt(Ye.REQUIRED_VALUE, "path");
         return e
     } else throw rt(Ye.INVALID_VALUE)
 }
 
-function cl(e) {
+function ll(e) {
     const {
         path: t,
         locale: n,
         args: r,
         choice: o,
         plural: a
     } = e, s = {}, u = r || {};
     return U(n) && (s.locale = n), Ce(o) && (s.plural = o), Ce(a) && (s.plural = a), [t, u, s]
 }
 
 function Pz(e, t, ...n) {
     const r = ae(n[0]) ? n[0] : {},
         o = !!r.useI18nComponentName;
-    (ge(r.globalInstall) ? r.globalInstall : !0) && (e.component(o ? "i18n" : il.name, il), e.component(al.name, al), e.component(sl.name, sl)), e.directive("t", Az(t))
+    (ge(r.globalInstall) ? r.globalInstall : !0) && (e.component(o ? "i18n" : ol.name, ol), e.component(il.name, il), e.component(al.name, al)), e.directive("t", Az(t))
 }
 const Ez = Ht("global-vue-i18n");
 
 function Mz(e = {}, t) {
     const n = ge(e.globalInjection) ? e.globalInjection : !0,
         r = !0,
         o = new Map,
@@ -11988,16 +11978,16 @@
             __setInstance: l,
             __deleteInstance: d
         };
         return m
     }
 }
 
-function ia(e = {}) {
-    const t = On();
+function oa(e = {}) {
+    const t = In();
     if (t == null) throw rt(Ye.MUST_BE_CALL_SETUP_TOP);
     if (!t.isCE && t.appContext.app != null && !t.appContext.app.__VUE_I18N_SYMBOL__) throw rt(Ye.NOT_INSLALLED);
     const n = Cz(t),
         r = Dz(n),
         o = Du(t),
         a = kz(e, o);
     if (a === "global") return gz(r, e, o), r;
@@ -12011,15 +12001,15 @@
         const c = Fe({}, e);
         "__i18n" in o && (c.__i18n = o.__i18n), r && (c.__root = r), u = Iu(c), Oz(s, t), s.__setInstance(t, u)
     }
     return u
 }
 
 function wz(e, t, n) {
-    const r = bl(); {
+    const r = zl(); {
         const o = r.run(() => Iu(e));
         if (o == null) throw rt(Ye.UNEXPECTED_ERROR);
         return [r, o]
     }
 }
 
 function Cz(e) {
@@ -12027,15 +12017,15 @@
         const t = ke(e.isCE ? Ez : e.appContext.app.__VUE_I18N_SYMBOL__);
         if (!t) throw rt(e.isCE ? Ye.NOT_INSLALLED_WITH_PROVIDE : Ye.UNEXPECTED_ERROR);
         return t
     }
 }
 
 function kz(e, t) {
-    return bo(e) ? "__i18n" in t ? "local" : "global" : e.useScope ? e.useScope : "local"
+    return zo(e) ? "__i18n" in t ? "local" : "global" : e.useScope ? e.useScope : "local"
 }
 
 function Dz(e) {
     return e.mode === "composition" ? e.global : e.global.__composer
 }
 
 function Iz(e, t, n = !1) {
@@ -12047,15 +12037,15 @@
         if (e.mode === "composition" && (r = s.__getInstance(a)), r != null || o === a) break;
         a = a.parent
     }
     return r
 }
 
 function Oz(e, t, n) {
-    io(() => {}, t), Li(() => {
+    oo(() => {}, t), Ri(() => {
         e.__deleteInstance(t)
     }, t)
 }
 const Gz = ["locale", "fallbackLocale", "availableLocales"],
     Rz = ["t", "rt", "d", "n", "tm"];
 
 function Lz(e, t) {
@@ -12082,15 +12072,15 @@
         Object.defineProperty(e.config.globalProperties, `$${r}`, o)
     })
 }
 az(Fh);
 sz(gu);
 hz();
 if (__INTLIFY_PROD_DEVTOOLS__) {
-    const e = Ji();
+    const e = Zi();
     e.__INTLIFY__ = !0, Yh(e.__INTLIFY_DEVTOOLS_GLOBAL_HOOK__)
 }
 const Bz = {
         da: {
             actions: e => {
                 const {
                     normalize: t
@@ -14983,14 +14973,86 @@
                     return t(["Core"])
                 },
                 core_modules: e => {
                     const {
                         normalize: t
                     } = e;
                     return t(["Core modules"])
+                },
+                server_info: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Server information"])
+                },
+                server_id: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Server ID"])
+                },
+                server_version: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Server version"])
+                },
+                server_base_url: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Base URL"])
+                },
+                server_as_addon: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Home Assistant add-on"])
+                },
+                artists_in_library: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Artists in library"])
+                },
+                albums_in_library: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Albums in library"])
+                },
+                tracks_in_library: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Tracks in library"])
+                },
+                playlists_in_library: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Playlists in library"])
+                },
+                radio_in_library: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Radio in library"])
+                },
+                server_logging: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Server logging"])
+                },
+                download_log: e => {
+                    const {
+                        normalize: t
+                    } = e;
+                    return t(["Download logfile"])
                 }
             },
             show_info: e => {
                 const {
                     normalize: t
                 } = e;
                 return t(["Show info"])
@@ -15286,14 +15348,26 @@
             check_item_in_library: e => {
                 const {
                     normalize: t,
                     interpolate: n,
                     list: r
                 } = e;
                 return t(["Check ", n(r(0)), " in the library"])
+            },
+            media_details: e => {
+                const {
+                    normalize: t
+                } = e;
+                return t(["Media details"])
+            },
+            mapped_providers: e => {
+                const {
+                    normalize: t
+                } = e;
+                return t(["Mapped providers"])
             }
         },
         es: {
             actions: e => {
                 const {
                     normalize: t
                 } = e;
@@ -22140,16 +22214,16 @@
         if (typeof window < "u") return function(n) {
             window.MobileDetect = n()
         };
         throw new Error("unknown environment")
     }())
 })(Ru);
 var xz = Ru.exports;
-const Fz = vc(xz),
-    En = new Fz(window.navigator.userAgent),
+const Fz = yc(xz),
+    Pn = new Fz(window.navigator.userAgent),
     Re = {
         bp0: 375,
         bp1: 500,
         bp2: 540,
         bp3: 575,
         bp4: 715,
         bp5: 800,
@@ -22167,55 +22241,55 @@
 });
 const Yb = e => {
         let t = "bp1",
             n = "gt",
             r = 0;
         if (typeof e == "object" ? (t = e.breakpoint, n = e.condition || "gt", r = e.offset || 0) : t = e, Object.values(["mobile", "phone", "tablet"]).includes(t)) switch (typeof e == "object" && (n = e.condition || "lt"), t) {
             case "mobile":
-                return En.mobile() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
+                return Pn.mobile() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
             case "phone":
-                return En.phone() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
+                return Pn.phone() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
             case "tablet":
-                return En.tablet() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3
+                return Pn.tablet() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3
         } else return n === "lt" ? ve.width < Re[t] + r : ve.width >= Re[t] + r;
         return !1
     },
-    ul = () => {
+    cl = () => {
         ve.width = window.innerWidth
     },
     Vz = {
         beforeMount(e, t) {
             let n = "gt",
                 r = "bp1",
                 o = 0;
             typeof t.value == "object" ? (n = t.value.condition, r = t.value.breakpoint, o = t.value.offset || 0) : r = t.value, Object.values(["mobile", "phone", "tablet"]).includes(r) && (n = t.value.condition || "lt");
             const a = u => {
-                    if (u === "mobile") return !!En.mobile() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
-                    if (u === "phone") return !!En.phone() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
-                    if (u === "tablet") return !!En.tablet() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3
+                    if (u === "mobile") return !!Pn.mobile() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
+                    if (u === "phone") return !!Pn.phone() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3;
+                    if (u === "tablet") return !!Pn.tablet() ? !0 : n === "lt" ? ve.width < Re.bp3 : ve.width >= Re.bp3
                 },
                 s = () => {
                     Object.values(["mobile", "phone", "tablet"]).includes(r) ? a(r) ? e.style.display = "" : e.style.display = "none" : (n === "lt" ? ve.width < Re[r] + o : ve.width >= Re[r] + o) ? e.style.display = "" : e.style.display = "none"
                 };
-            window.addEventListener("resize", ul), xe(() => ve.width, s), s(), e._onDestroy = () => {
-                window.removeEventListener("resize", ul)
+            window.addEventListener("resize", cl), xe(() => ve.width, s), s(), e._onDestroy = () => {
+                window.removeEventListener("resize", cl)
             }
         },
         unmounted(e) {
             e._onDestroy()
         }
     },
     Uz = {
         install(e) {
-            e.config.globalProperties.$screenSize = ki(ve), e.directive("breakpoint", Vz)
+            e.config.globalProperties.$screenSize = Ci(ve), e.directive("breakpoint", Vz)
         }
     };
 
 function Wz(e) {
     e.use(gp).use(_u).use(Nz).use(Hz).use(Uz)
 }
 const Lu = gf(Q0);
 Wz(Lu);
 Lu.mount("#app");
 export {
-    Jf as $, lt as A, ut as B, vb as C, Yb as D, u_ as E, He as F, Ec as G, to as H, $b as I, ia as J, Cd as K, cc as L, ab as M, qz as N, Yo as O, ad as P, Qz as Q, Zz as R, Vb as S, fc as T, Yf as U, tb as V, Ti as W, vi as X, nb as Y, Xb as Z, _n as _, fb as a, Db as a$, Pc as a0, jb as a1, vs as a2, gp as a3, _u as a4, Xz as a5, $z as a6, Ub as a7, Kb as a8, Jz as a9, Zf as aA, Gb as aB, ur as aC, rn as aD, Yz as aE, Il as aF, Cl as aG, rb as aH, bb as aI, cb as aJ, fn as aK, yt as aL, __ as aM, t_ as aN, n_ as aO, mb as aP, yb as aQ, Cc as aR, hb as aS, c_ as aT, tm as aU, gb as aV, Ob as aW, Eb as aX, Ab as aY, Nt as aZ, wb as a_, Qf as aa, On as ab, pe as ac, r_ as ad, Wb as ae, at as af, e_ as ag, qb as ah, lb as ai, Fb as aj, ke as ak, Lc as al, on as am, Pn as an, Qm as ao, Ym as ap, Xe as aq, ko as ar, zb as as, ki as at, Li as au, N_ as av, Bb as aw, o0 as ax, kc as ay, ub as az, Yl as b, Pb as b0, kl as b1, dr as b2, db as b3, p_ as b4, Tb as b5, bl as b6, _b as b7, ee as b8, ob as b9, gt as ba, Ib as bb, Cb as bc, sb as bd, Sb as be, Ae as bf, kb as bg, Lb as bh, d_ as bi, mr as bj, Mb as bk, Ya as bl, pb as bm, re as c, xb as d, Rb as e, W_ as f, C_ as g, Jm as h, O_ as i, fe as j, uc as k, no as l, Hb as m, Ii as n, io as o, $i as p, Vi as q, Me as r, Jt as s, Kz as t, Nb as u, Ui as v, xe as w, Ul as x, ib as y, eb as z
+    Jf as $, lt as A, ut as B, vb as C, Yb as D, u_ as E, He as F, Ec as G, eo as H, $b as I, oa as J, Cd as K, lc as L, ab as M, qz as N, $o as O, ad as P, Qz as Q, Zz as R, Yf as S, dc as T, Vb as U, tb as V, vi as W, yi as X, nb as Y, Xb as Z, fn as _, fb as a, Db as a$, Pc as a0, jb as a1, ys as a2, gp as a3, _u as a4, Xz as a5, $z as a6, Ub as a7, Kb as a8, Jz as a9, Zf as aA, Gb as aB, cr as aC, rn as aD, Yz as aE, Dl as aF, wl as aG, rb as aH, bb as aI, cb as aJ, Ac as aK, yt as aL, __ as aM, t_ as aN, n_ as aO, mb as aP, yb as aQ, Cc as aR, hb as aS, c_ as aT, tm as aU, gb as aV, Ob as aW, Eb as aX, Ab as aY, Nt as aZ, wb as a_, Qf as aa, In as ab, pe as ac, r_ as ad, Wb as ae, at as af, e_ as ag, lb as ah, qb as ai, Fb as aj, ke as ak, Lc as al, on as am, An as an, Qm as ao, Ym as ap, Xe as aq, Co as ar, zb as as, Ci as at, Ri as au, N_ as av, Bb as aw, o0 as ax, kc as ay, ub as az, $l as b, Pb as b0, Cl as b1, mr as b2, db as b3, p_ as b4, Tb as b5, zl as b6, _b as b7, ee as b8, ob as b9, gt as ba, Ib as bb, Cb as bc, sb as bd, Sb as be, Ae as bf, kb as bg, Lb as bh, d_ as bi, ur as bj, Mb as bk, $a as bl, pb as bm, re as c, xb as d, Rb as e, W_ as f, C_ as g, Jm as h, O_ as i, fe as j, cc as k, to as l, Hb as m, Di as n, oo as o, Xi as p, Fi as q, Me as r, Jt as s, Kz as t, Nb as u, Vi as v, xe as w, Vl as x, ib as y, eb as z
 };
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/index-ecb9e627.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/index-ecb9e627.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/layout-4499d5bc.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/layout-b0232ef9.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     n as ee
-} from "./VBtn-68784d55.js";
+} from "./VBtn-61e39030.js";
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
-} from "./index-e9211ef1.js";
+} from "./index-ade73b84.js";
 const M = Symbol.for("vuetify:layout"),
     D = Symbol.for("vuetify:layout-item"),
     K = 1e3,
     de = N({
         overlaps: {
             type: Array,
             default: () => []
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/logo-c9d5d6ab.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/logo-c9d5d6ab.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/m4a-45331b05.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/m4a-45331b05.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/vue-virtual-scroller-4d71315f.css`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/assets/workbox-window.prod.es5-a7b12eab.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/favicon.ico` & `music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/favicon.svg` & `music-assistant-frontend-2.0.4/music_assistant_frontend/favicon.svg`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/index.html` & `music-assistant-frontend-2.0.4/music_assistant_frontend/index.html`

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
-    <script type="module" crossorigin src="./assets/index-e9211ef1.js"></script>
+    <script type="module" crossorigin src="./assets/index-ade73b84.js"></script>
     <link rel="stylesheet" href="./assets/index-ecb9e627.css">
   <link rel="manifest" href="./manifest.webmanifest"><style>@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:100;font-display:swap;src:url(./assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCRc4EsA-435e4b7f.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fABc4EsA-47aa3bfa.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCBc4EsA-20dc200c.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBxc4EsA-455c2c1a.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fCxc4EsA-51f3f418.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fChc4EsA-b076e863.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:300;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmSU5fBBc4-f7591131.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:400;font-display:swap;src:url(./assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCRc4EsA-aeed0e51.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fABc4EsA-3728fbdd.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCBc4EsA-ef8f0236.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBxc4EsA-713780d8.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fCxc4EsA-0948409a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fChc4EsA-7f1c829b.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:500;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmEU9fBBc4-b0195382.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCRc4EsA-3c505383.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfABc4EsA-6a84eeee.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCBc4EsA-5b6377da.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBxc4EsA-1c9cc76f.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfCxc4EsA-4ec57f2a.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfChc4EsA-fc66f942.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:700;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmWUlfBBc4-f5aebdfe.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCRc4EsA-f265cee6.woff2) format('woff2');unicode-range:U+0460-052F,U+1C80-1C88,U+20B4,U+2DE0-2DFF,U+A640-A69F,U+FE2E-FE2F}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfABc4EsA-9fdb12ce.woff2) format('woff2');unicode-range:U+0301,U+0400-045F,U+0490-0491,U+04B0-04B1,U+2116}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCBc4EsA-76da333a.woff2) format('woff2');unicode-range:U+1F00-1FFF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBxc4EsA-2550c2e2.woff2) format('woff2');unicode-range:U+0370-03FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfCxc4EsA-3a38c967.woff2) format('woff2');unicode-range:U+0102-0103,U+0110-0111,U+0128-0129,U+0168-0169,U+01A0-01A1,U+01AF-01B0,U+0300-0301,U+0303-0304,U+0308-0309,U+0323,U+0329,U+1EA0-1EF9,U+20AB}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfChc4EsA-2781e9e7.woff2) format('woff2');unicode-range:U+0100-02AF,U+0304,U+0308,U+0329,U+1E00-1E9F,U+1EF2-1EFF,U+2020,U+20A0-20AB,U+20AD-20CF,U+2113,U+2C60-2C7F,U+A720-A7FF}@font-face{font-family:Roboto;font-style:normal;font-weight:900;font-display:swap;src:url(./assets/KFOlCnqEu92Fr1MmYUtfBBc4-7e262106.woff2) format('woff2');unicode-range:U+0000-00FF,U+0131,U+0152-0153,U+02BB-02BC,U+02C6,U+02DA,U+02DC,U+0304,U+0308,U+0329,U+2000-206F,U+2074,U+20AC,U+2122,U+2191,U+2193,U+2212,U+2215,U+FEFF,U+FFFD}</style></head>
   <body>
     <noscript>
       <strong
         >We're sorry but musicassistant-frontend doesn't work properly without
         JavaScript enabled. Please enable it to continue.</strong
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/manifest.webmanifest` & `music-assistant-frontend-2.0.4/music_assistant_frontend/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/pwa-192x192.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-192x192.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/pwa-512x512.png` & `music-assistant-frontend-2.0.4/music_assistant_frontend/pwa-512x512.png`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/sw.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/sw.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -26,241 +26,244 @@
     }
 }
 define(["./workbox-27b29e6f"], (function(s) {
     "use strict";
     self.addEventListener("message", (s => {
         s.data && "SKIP_WAITING" === s.data.type && self.skipWaiting()
     })), s.precacheAndRoute([{
-        url: "assets/AddProvider-32056ca3.js",
+        url: "assets/AddProvider-a95ca786.js",
         revision: null
     }, {
-        url: "assets/AlbumDetails-343f22cb.js",
+        url: "assets/AlbumDetails-55ac33a4.js",
         revision: null
     }, {
-        url: "assets/Alert-55091fd0.js",
+        url: "assets/Alert-4d78da02.js",
         revision: null
     }, {
         url: "assets/Alert-c80b13d7.css",
         revision: null
     }, {
-        url: "assets/ArtistDetails-7bca6a8e.js",
+        url: "assets/ArtistDetails-7c7516d2.js",
         revision: null
     }, {
-        url: "assets/BrowseView-d63a1e11.js",
+        url: "assets/BrowseView-457188ac.js",
         revision: null
     }, {
         url: "assets/Button-15e2fa72.css",
         revision: null
     }, {
-        url: "assets/Button-59559304.js",
+        url: "assets/Button-4a781169.js",
         revision: null
     }, {
-        url: "assets/Container-349a0ac0.js",
+        url: "assets/Container-282a676b.js",
         revision: null
     }, {
         url: "assets/Container-ed1c67df.css",
         revision: null
     }, {
-        url: "assets/CoreConfigs-0b98268a.js",
+        url: "assets/CoreConfigs-1c0e2549.css",
         revision: null
     }, {
-        url: "assets/Default-27a728f1.js",
+        url: "assets/CoreConfigs-69940384.js",
+        revision: null
+    }, {
+        url: "assets/Default-4e51f0b8.js",
         revision: null
     }, {
         url: "assets/Default-8766b49d.css",
         revision: null
     }, {
         url: "assets/EditConfig-25e44c20.css",
         revision: null
     }, {
-        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js",
+        url: "assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js",
         revision: null
     }, {
-        url: "assets/EditCoreConfig-d3e464b0.js",
+        url: "assets/EditCoreConfig-714d074a.js",
         revision: null
     }, {
-        url: "assets/EditPlayer-19592b08.js",
+        url: "assets/EditPlayer-f0c55a15.js",
         revision: null
     }, {
-        url: "assets/EditProvider-019f1e2b.js",
+        url: "assets/EditProvider-a2553a06.js",
         revision: null
     }, {
-        url: "assets/HomeView-6873693d.js",
+        url: "assets/HomeView-af5707e7.js",
         revision: null
     }, {
         url: "assets/HomeView-f559b858.css",
         revision: null
     }, {
-        url: "assets/index-e9211ef1.js",
+        url: "assets/index-ade73b84.js",
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
-        url: "assets/InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js",
+        url: "assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js",
         revision: null
     }, {
         url: "assets/ItemsListing-7290acd0.css",
         revision: null
     }, {
-        url: "assets/ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js",
+        url: "assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js",
         revision: null
     }, {
-        url: "assets/layout-4499d5bc.js",
+        url: "assets/layout-b0232ef9.js",
         revision: null
     }, {
-        url: "assets/LibraryAlbums-ea4898eb.js",
+        url: "assets/LibraryAlbums-757b8aa2.js",
         revision: null
     }, {
-        url: "assets/LibraryArtists-be1957cb.js",
+        url: "assets/LibraryArtists-225ce0c1.js",
         revision: null
     }, {
-        url: "assets/LibraryPlaylists-a9b54924.js",
+        url: "assets/LibraryPlaylists-4ffdc19f.js",
         revision: null
     }, {
-        url: "assets/LibraryRadios-996c89ba.js",
+        url: "assets/LibraryRadios-a948d358.js",
         revision: null
     }, {
-        url: "assets/LibraryTracks-d64430e5.js",
+        url: "assets/LibraryTracks-5a540fa3.js",
         revision: null
     }, {
-        url: "assets/ListviewItem-9fa6da34.css",
+        url: "assets/ListviewItem-2bd74fad.js",
         revision: null
     }, {
-        url: "assets/ListviewItem-b7a4258b.js",
+        url: "assets/ListviewItem-732a7603.css",
         revision: null
     }, {
         url: "assets/MediaItemThumb-24a77af5.css",
         revision: null
     }, {
-        url: "assets/MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js",
+        url: "assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js",
         revision: null
     }, {
         url: "assets/PanelviewItem-14a6b77a.css",
         revision: null
     }, {
-        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js",
+        url: "assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js",
         revision: null
     }, {
-        url: "assets/PlayerQueue-29876489.js",
+        url: "assets/PlayerQueue-7ca94b07.js",
         revision: null
     }, {
-        url: "assets/Players-b1f01106.js",
+        url: "assets/Players-5c99fe5e.js",
         revision: null
     }, {
-        url: "assets/PlaylistDetails-09b11191.js",
+        url: "assets/PlaylistDetails-f8a1c191.js",
         revision: null
     }, {
         url: "assets/Providers-0e527c0c.css",
         revision: null
     }, {
-        url: "assets/Providers-a361876b.js",
+        url: "assets/Providers-65d3d824.js",
         revision: null
     }, {
-        url: "assets/RadioDetails-6f742445.js",
+        url: "assets/RadioDetails-71dc877e.js",
         revision: null
     }, {
-        url: "assets/Search-b8c39f87.js",
+        url: "assets/Search-f31ee239.js",
         revision: null
     }, {
-        url: "assets/Settings-244fcb0f.js",
+        url: "assets/Settings-f159e60c.js",
         revision: null
     }, {
-        url: "assets/TrackDetails-71587bd7.js",
+        url: "assets/TrackDetails-ca02e9b2.js",
         revision: null
     }, {
-        url: "assets/VBadge-9c063078.css",
+        url: "assets/VBadge-12aff0c7.js",
         revision: null
     }, {
-        url: "assets/VBadge-9fa94f29.js",
+        url: "assets/VBadge-9c063078.css",
         revision: null
     }, {
-        url: "assets/VBtn-68784d55.js",
+        url: "assets/VBtn-61e39030.js",
         revision: null
     }, {
         url: "assets/VBtn-76f512af.css",
         revision: null
     }, {
         url: "assets/VCard-103d8462.css",
         revision: null
     }, {
-        url: "assets/VCard-138864fc.js",
+        url: "assets/VCard-f3e11b51.js",
         revision: null
     }, {
         url: "assets/VDialog-28e4e64e.css",
         revision: null
     }, {
-        url: "assets/VDialog-5f240a62.js",
+        url: "assets/VDialog-93a2100b.js",
         revision: null
     }, {
-        url: "assets/VDivider-336c24cd.js",
+        url: "assets/VDivider-adefbf87.js",
         revision: null
     }, {
         url: "assets/VDivider-bc1524a3.css",
         revision: null
     }, {
         url: "assets/VExpansionPanel-16e67e58.css",
         revision: null
     }, {
-        url: "assets/VExpansionPanel-67038b00.js",
+        url: "assets/VExpansionPanel-75456689.js",
         revision: null
     }, {
         url: "assets/VGrid-b9c72806.css",
         revision: null
     }, {
-        url: "assets/VListItem-230d1393.js",
+        url: "assets/VListItem-b9e24cb0.css",
         revision: null
     }, {
-        url: "assets/VListItem-b9e24cb0.css",
+        url: "assets/VListItem-f848c028.js",
         revision: null
     }, {
         url: "assets/VMenu-b930657a.css",
         revision: null
     }, {
-        url: "assets/VMenu-bc0cce60.js",
+        url: "assets/VMenu-ccc026f2.js",
         revision: null
     }, {
-        url: "assets/VRow-e8f3e51e.js",
+        url: "assets/VRow-74a0e5a5.js",
         revision: null
     }, {
-        url: "assets/VSelect-04a129eb.js",
+        url: "assets/VSelect-45a454b3.css",
         revision: null
     }, {
-        url: "assets/VSelect-45a454b3.css",
+        url: "assets/VSelect-a66ffc02.js",
         revision: null
     }, {
-        url: "assets/VSpacer-bdf2f653.js",
+        url: "assets/VSpacer-159b0383.js",
         revision: null
     }, {
-        url: "assets/VTabs-13127e50.js",
+        url: "assets/VTabs-21d8affa.js",
         revision: null
     }, {
         url: "assets/VTabs-3cd3e980.css",
         revision: null
     }, {
         url: "assets/VToolbar-222d6375.css",
         revision: null
     }, {
-        url: "assets/VToolbar-daf2b89f.js",
+        url: "assets/VToolbar-806969a3.js",
         revision: null
     }, {
         url: "assets/vue-virtual-scroller-4d71315f.css",
         revision: null
     }, {
         url: "assets/workbox-window.prod.es5-a7b12eab.js",
         revision: null
     }, {
         url: "index.html",
-        revision: "978305765ffbf6d9f4e0c00b44c96dcc"
+        revision: "fbf1a9e0c6d1935e8ef5886fdff83bbf"
     }, {
         url: "favicon.svg",
         revision: "ecfda4076e793b6ffd619ed24e66c36d"
     }, {
         url: "favicon.ico",
         revision: "60d77c1713c2255be3f6de69c4de24d9"
     }, {
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend/workbox-27b29e6f.js` & `music-assistant-frontend-2.0.4/music_assistant_frontend/workbox-27b29e6f.js`

 * *Files identical despite different names*

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/PKG-INFO` & `music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-assistant-frontend
-Version: 2.0.3
+Version: 2.0.4
 Summary: The Music Assistant frontend
 Author-email: The Music Assistant Authors <m.vanderveldt@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/music-assistant/frontend
 Platform: any
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
```

### Comparing `music-assistant-frontend-2.0.3/music_assistant_frontend.egg-info/SOURCES.txt` & `music-assistant-frontend-2.0.4/music_assistant_frontend.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,38 +16,39 @@
 music_assistant_frontend/sw.js
 music_assistant_frontend/workbox-27b29e6f.js
 music_assistant_frontend.egg-info/PKG-INFO
 music_assistant_frontend.egg-info/SOURCES.txt
 music_assistant_frontend.egg-info/dependency_links.txt
 music_assistant_frontend.egg-info/not-zip-safe
 music_assistant_frontend.egg-info/top_level.txt
-music_assistant_frontend/assets/AddProvider-32056ca3.js
-music_assistant_frontend/assets/AlbumDetails-343f22cb.js
-music_assistant_frontend/assets/Alert-55091fd0.js
+music_assistant_frontend/assets/AddProvider-a95ca786.js
+music_assistant_frontend/assets/AlbumDetails-55ac33a4.js
+music_assistant_frontend/assets/Alert-4d78da02.js
 music_assistant_frontend/assets/Alert-c80b13d7.css
-music_assistant_frontend/assets/ArtistDetails-7bca6a8e.js
-music_assistant_frontend/assets/BrowseView-d63a1e11.js
+music_assistant_frontend/assets/ArtistDetails-7c7516d2.js
+music_assistant_frontend/assets/BrowseView-457188ac.js
 music_assistant_frontend/assets/Button-15e2fa72.css
-music_assistant_frontend/assets/Button-59559304.js
-music_assistant_frontend/assets/Container-349a0ac0.js
+music_assistant_frontend/assets/Button-4a781169.js
+music_assistant_frontend/assets/Container-282a676b.js
 music_assistant_frontend/assets/Container-ed1c67df.css
-music_assistant_frontend/assets/CoreConfigs-0b98268a.js
-music_assistant_frontend/assets/Default-27a728f1.js
+music_assistant_frontend/assets/CoreConfigs-1c0e2549.css
+music_assistant_frontend/assets/CoreConfigs-69940384.js
+music_assistant_frontend/assets/Default-4e51f0b8.js
 music_assistant_frontend/assets/Default-8766b49d.css
 music_assistant_frontend/assets/EditConfig-25e44c20.css
-music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-29ce80f7.js
-music_assistant_frontend/assets/EditCoreConfig-d3e464b0.js
-music_assistant_frontend/assets/EditPlayer-19592b08.js
-music_assistant_frontend/assets/EditProvider-019f1e2b.js
-music_assistant_frontend/assets/HomeView-6873693d.js
+music_assistant_frontend/assets/EditConfig.vue_vue_type_style_index_0_lang-9825e058.js
+music_assistant_frontend/assets/EditCoreConfig-714d074a.js
+music_assistant_frontend/assets/EditPlayer-f0c55a15.js
+music_assistant_frontend/assets/EditProvider-a2553a06.js
+music_assistant_frontend/assets/HomeView-af5707e7.js
 music_assistant_frontend/assets/HomeView-f559b858.css
 music_assistant_frontend/assets/InfoHeader-32cd2df9.css
-music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-36a95710.js
+music_assistant_frontend/assets/InfoHeader.vue_vue_type_style_index_0_lang-2f9c70b4.js
 music_assistant_frontend/assets/ItemsListing-7290acd0.css
-music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-436cf3d3.js
+music_assistant_frontend/assets/ItemsListing.vue_vue_type_script_setup_true_lang-3b792876.js
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxEIzIFKw-8007dfe8.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxFIzIFKw-8e48cf20.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxGIzIFKw-10b31f4c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxHIzIFKw-ca7eea0c.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxIIzI-0f303f31.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxLIzIFKw-8c3798e3.woff2
 music_assistant_frontend/assets/KFOkCnqEu92Fr1MmgVxMIzIFKw-638764dc.woff2
@@ -82,72 +83,72 @@
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4WxKOzY-daf51ab5.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu4mxK-f6734f81.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu5mxKOzY-495d38d4.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu72xKOzY-b7ef2cd1.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7GxKOzY-3c23eb02.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7WxKOzY-77b24796.woff2
 music_assistant_frontend/assets/KFOmCnqEu92Fr1Mu7mxKOzY-d368cf5b.woff2
-music_assistant_frontend/assets/LibraryAlbums-ea4898eb.js
-music_assistant_frontend/assets/LibraryArtists-be1957cb.js
-music_assistant_frontend/assets/LibraryPlaylists-a9b54924.js
-music_assistant_frontend/assets/LibraryRadios-996c89ba.js
-music_assistant_frontend/assets/LibraryTracks-d64430e5.js
-music_assistant_frontend/assets/ListviewItem-9fa6da34.css
-music_assistant_frontend/assets/ListviewItem-b7a4258b.js
+music_assistant_frontend/assets/LibraryAlbums-757b8aa2.js
+music_assistant_frontend/assets/LibraryArtists-225ce0c1.js
+music_assistant_frontend/assets/LibraryPlaylists-4ffdc19f.js
+music_assistant_frontend/assets/LibraryRadios-a948d358.js
+music_assistant_frontend/assets/LibraryTracks-5a540fa3.js
+music_assistant_frontend/assets/ListviewItem-2bd74fad.js
+music_assistant_frontend/assets/ListviewItem-732a7603.css
 music_assistant_frontend/assets/MaterialIcons-Regular-11ec382a.woff
 music_assistant_frontend/assets/MaterialIcons-Regular-29c11fa5.ttf
 music_assistant_frontend/assets/MaterialIcons-Regular-5743ed3d.woff2
 music_assistant_frontend/assets/MaterialIcons-Regular-e69d687a.eot
 music_assistant_frontend/assets/MediaItemThumb-24a77af5.css
-music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-278977b5.js
+music_assistant_frontend/assets/MediaItemThumb.vue_vue_type_style_index_0_lang-cd169f56.js
 music_assistant_frontend/assets/PanelviewItem-14a6b77a.css
-music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-fefd2afe.js
-music_assistant_frontend/assets/PlayerQueue-29876489.js
-music_assistant_frontend/assets/Players-b1f01106.js
-music_assistant_frontend/assets/PlaylistDetails-09b11191.js
+music_assistant_frontend/assets/PanelviewItem.vue_vue_type_style_index_0_lang-93dbfb68.js
+music_assistant_frontend/assets/PlayerQueue-7ca94b07.js
+music_assistant_frontend/assets/Players-5c99fe5e.js
+music_assistant_frontend/assets/PlaylistDetails-f8a1c191.js
 music_assistant_frontend/assets/Providers-0e527c0c.css
-music_assistant_frontend/assets/Providers-a361876b.js
-music_assistant_frontend/assets/RadioDetails-6f742445.js
-music_assistant_frontend/assets/Search-b8c39f87.js
-music_assistant_frontend/assets/Settings-244fcb0f.js
-music_assistant_frontend/assets/TrackDetails-71587bd7.js
+music_assistant_frontend/assets/Providers-65d3d824.js
+music_assistant_frontend/assets/RadioDetails-71dc877e.js
+music_assistant_frontend/assets/Search-f31ee239.js
+music_assistant_frontend/assets/Settings-f159e60c.js
+music_assistant_frontend/assets/TrackDetails-ca02e9b2.js
+music_assistant_frontend/assets/VBadge-12aff0c7.js
 music_assistant_frontend/assets/VBadge-9c063078.css
-music_assistant_frontend/assets/VBadge-9fa94f29.js
-music_assistant_frontend/assets/VBtn-68784d55.js
+music_assistant_frontend/assets/VBtn-61e39030.js
 music_assistant_frontend/assets/VBtn-76f512af.css
 music_assistant_frontend/assets/VCard-103d8462.css
-music_assistant_frontend/assets/VCard-138864fc.js
+music_assistant_frontend/assets/VCard-f3e11b51.js
 music_assistant_frontend/assets/VDialog-28e4e64e.css
-music_assistant_frontend/assets/VDialog-5f240a62.js
-music_assistant_frontend/assets/VDivider-336c24cd.js
+music_assistant_frontend/assets/VDialog-93a2100b.js
+music_assistant_frontend/assets/VDivider-adefbf87.js
 music_assistant_frontend/assets/VDivider-bc1524a3.css
 music_assistant_frontend/assets/VExpansionPanel-16e67e58.css
-music_assistant_frontend/assets/VExpansionPanel-67038b00.js
+music_assistant_frontend/assets/VExpansionPanel-75456689.js
 music_assistant_frontend/assets/VGrid-b9c72806.css
-music_assistant_frontend/assets/VListItem-230d1393.js
 music_assistant_frontend/assets/VListItem-b9e24cb0.css
+music_assistant_frontend/assets/VListItem-f848c028.js
 music_assistant_frontend/assets/VMenu-b930657a.css
-music_assistant_frontend/assets/VMenu-bc0cce60.js
-music_assistant_frontend/assets/VRow-e8f3e51e.js
-music_assistant_frontend/assets/VSelect-04a129eb.js
+music_assistant_frontend/assets/VMenu-ccc026f2.js
+music_assistant_frontend/assets/VRow-74a0e5a5.js
 music_assistant_frontend/assets/VSelect-45a454b3.css
-music_assistant_frontend/assets/VSpacer-bdf2f653.js
-music_assistant_frontend/assets/VTabs-13127e50.js
+music_assistant_frontend/assets/VSelect-a66ffc02.js
+music_assistant_frontend/assets/VSpacer-159b0383.js
+music_assistant_frontend/assets/VTabs-21d8affa.js
 music_assistant_frontend/assets/VTabs-3cd3e980.css
 music_assistant_frontend/assets/VToolbar-222d6375.css
-music_assistant_frontend/assets/VToolbar-daf2b89f.js
+music_assistant_frontend/assets/VToolbar-806969a3.js
 music_assistant_frontend/assets/cover_dark-75402cd0.png
 music_assistant_frontend/assets/cover_light-b832ae9e.png
 music_assistant_frontend/assets/crossfade-ba51f69a.png
 music_assistant_frontend/assets/hires-438c7046.png
-music_assistant_frontend/assets/index-e9211ef1.js
+music_assistant_frontend/assets/index-ade73b84.js
 music_assistant_frontend/assets/index-ecb9e627.css
 music_assistant_frontend/assets/index.browser-7e542916.js
 music_assistant_frontend/assets/info_gradient-a4aefd1d.jpg
-music_assistant_frontend/assets/layout-4499d5bc.js
+music_assistant_frontend/assets/layout-b0232ef9.js
 music_assistant_frontend/assets/logo-c9d5d6ab.png
 music_assistant_frontend/assets/m4a-45331b05.png
 music_assistant_frontend/assets/material-icons-outlined-35dca8a7.woff2
 music_assistant_frontend/assets/materialdesignicons-webfont-67d24abe.eot
 music_assistant_frontend/assets/materialdesignicons-webfont-80bb28b3.woff
 music_assistant_frontend/assets/materialdesignicons-webfont-a58ecb54.ttf
 music_assistant_frontend/assets/materialdesignicons-webfont-c1c004a9.woff2
```

### Comparing `music-assistant-frontend-2.0.3/pyproject.toml` & `music-assistant-frontend-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools~=62.3",
     "wheel~=0.37.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "music-assistant-frontend"
-version = "2.0.3"
+version = "2.0.4"
 description = "The Music Assistant frontend"
 readme = "README.md"
 authors = [
     { name = "The Music Assistant Authors", email = "m.vanderveldt@outlook.com" },
 ]
 requires-python = ">=3.9.0"
```

