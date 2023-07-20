# Comparing `tmp/reflex-0.2.1a2.tar.gz` & `tmp/reflex-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.1a2.tar", max compression
+gzip compressed data, was "reflex-0.2.2a1.tar", max compression
```

## Comparing `reflex-0.2.1a2.tar` & `reflex-0.2.2a1.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.1a2/LICENSE
--rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.1a2/README.md
--rw-r--r--   0        0        0     2002 2023-07-19 01:58:40.554124 reflex-0.2.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.1a2/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.1a2/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.1a2/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.1a2/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.1a2/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.1a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.1a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.1a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.1a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.1a2/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.1a2/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.1a2/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.1a2/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1209 2023-07-19 01:58:26.537471 reflex-0.2.1a2/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.1a2/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.1a2/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.1a2/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.1a2/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.1a2/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10096 2023-07-19 01:58:26.537790 reflex-0.2.1a2/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.1a2/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.1a2/reflex/admin.py
--rw-r--r--   0        0        0    23515 2023-07-19 01:58:26.539090 reflex-0.2.1a2/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.1a2/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.1a2/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.1a2/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.1a2/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.1a2/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.1a2/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.1a2/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.1a2/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.1a2/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.1a2/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.1a2/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.1a2/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.1a2/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.1a2/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.1a2/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.1a2/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.1a2/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.1a2/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.1a2/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.1a2/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.1a2/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.1a2/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.1a2/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5762 2023-07-19 01:58:26.540483 reflex-0.2.1a2/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.1a2/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.1a2/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.1a2/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.1a2/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.1a2/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.1a2/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.1a2/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.1a2/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.1a2/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.1a2/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.1a2/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.1a2/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.1a2/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.1a2/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.1a2/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.1a2/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.1a2/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.1a2/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.1a2/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.1a2/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.1a2/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.1a2/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.1a2/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.1a2/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.1a2/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.1a2/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.1a2/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.1a2/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.1a2/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.1a2/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.1a2/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.1a2/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.1a2/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.1a2/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.1a2/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.1a2/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.1a2/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.1a2/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.1a2/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.1a2/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.1a2/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.1a2/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.1a2/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.1a2/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.1a2/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.1a2/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.1a2/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.1a2/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.1a2/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.1a2/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.1a2/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.1a2/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.1a2/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.1a2/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.1a2/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.1a2/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.1a2/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.1a2/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.1a2/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.1a2/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.1a2/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.1a2/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.1a2/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.1a2/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.1a2/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.1a2/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.1a2/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.1a2/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.1a2/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.1a2/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.1a2/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.1a2/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.1a2/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.1a2/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.1a2/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.1a2/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.1a2/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.1a2/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.1a2/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.1a2/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2294 2023-07-14 23:13:37.779060 reflex-0.2.1a2/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.1a2/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.1a2/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.1a2/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.1a2/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.1a2/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.1a2/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.1a2/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.1a2/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7215 2023-07-14 23:13:37.779630 reflex-0.2.1a2/reflex/config.py
--rw-r--r--   0        0        0    10821 2023-07-17 23:29:33.627808 reflex-0.2.1a2/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.1a2/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.1a2/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.1a2/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.1a2/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.1a2/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.1a2/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.1a2/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.1a2/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.1a2/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.1a2/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.1a2/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.1a2/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9473 2023-07-18 01:07:12.549028 reflex-0.2.1a2/reflex/model.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.1a2/reflex/py.typed
--rw-r--r--   0        0        0    11041 2023-07-19 01:58:26.540979 reflex-0.2.1a2/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.1a2/reflex/route.py
--rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.1a2/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.1a2/reflex/style.py
--rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.1a2/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.1a2/reflex/utils/__init__.py
--rw-r--r--   0        0        0     8232 2023-07-19 01:58:26.541268 reflex-0.2.1a2/reflex/utils/build.py
--rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.1a2/reflex/utils/console.py
--rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.1a2/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.1a2/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.1a2/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.1a2/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    14056 2023-07-19 01:58:26.541782 reflex-0.2.1a2/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.1a2/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.1a2/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.1a2/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.1a2/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-14 23:13:37.782718 reflex-0.2.1a2/reflex/vars.py
--rw-r--r--   0        0        0     9586 1970-01-01 00:00:00.000000 reflex-0.2.1a2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.2a1/LICENSE
+-rw-r--r--   0        0        0     7766 2023-07-17 23:29:33.625723 reflex-0.2.2a1/README.md
+-rw-r--r--   0        0        0     2002 2023-07-20 20:03:43.742215 reflex-0.2.2a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.2a1/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-19 01:58:23.983993 reflex-0.2.2a1/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.2a1/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.2a1/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.2a1/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.2a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.2a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.2a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.2a1/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.2a1/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.2a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-14 23:13:37.771678 reflex-0.2.2a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-20 20:03:35.347093 reflex-0.2.2a1/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-14 23:13:37.771821 reflex-0.2.2a1/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.2a1/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.2a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.2a1/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.2a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10110 2023-07-20 20:03:35.347375 reflex-0.2.2a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.2a1/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.2a1/reflex/admin.py
+-rw-r--r--   0        0        0    23767 2023-07-20 20:03:35.348327 reflex-0.2.2a1/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.2a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.2a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.2a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-14 23:13:37.772848 reflex-0.2.2a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.2a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.2a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.2a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.2a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.2a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.2a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.2a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.2a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.2a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.2a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-14 23:13:37.773563 reflex-0.2.2a1/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.2a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.2a1/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-14 23:13:37.773785 reflex-0.2.2a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-07-14 23:13:37.773859 reflex-0.2.2a1/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.2a1/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.2a1/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.2a1/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.2a1/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.2a1/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.2a1/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.2a1/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.2a1/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.2a1/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.2a1/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.2a1/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.2a1/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.2a1/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.2a1/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.2a1/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.2a1/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.2a1/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.2a1/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.2a1/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.2a1/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.2a1/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.2a1/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.2a1/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.2a1/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.2a1/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.2a1/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.2a1/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.2a1/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.2a1/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-14 23:13:37.775648 reflex-0.2.2a1/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.2a1/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.2a1/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.2a1/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.2a1/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.2a1/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.2a1/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.2a1/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.2a1/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.2a1/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.2a1/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.2a1/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.2a1/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.2a1/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.2a1/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.2a1/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.2a1/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.2a1/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.2a1/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.2a1/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.2a1/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.2a1/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.2a1/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-14 23:13:37.777060 reflex-0.2.2a1/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.2a1/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.2a1/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.2a1/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.2a1/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.2a1/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.2a1/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.2a1/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.2a1/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.2a1/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.2a1/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.2a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.2a1/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.2a1/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.2a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.2a1/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.2a1/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.2a1/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.2a1/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.2a1/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.2a1/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.2a1/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.2a1/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.2a1/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.2a1/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.2a1/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.2a1/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.2a1/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.2a1/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.2a1/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.2a1/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.2a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.2a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-20 20:03:37.472790 reflex-0.2.2a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-07-14 23:13:37.779125 reflex-0.2.2a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.2a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.2a1/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-14 23:13:37.779315 reflex-0.2.2a1/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.2a1/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3593 2023-07-14 23:13:37.779432 reflex-0.2.2a1/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.2a1/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.2a1/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7692 2023-07-20 20:03:35.349661 reflex-0.2.2a1/reflex/config.py
+-rw-r--r--   0        0        0    11103 2023-07-20 20:03:35.349925 reflex-0.2.2a1/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.2a1/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.2a1/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.2a1/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.2a1/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.2a1/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.2a1/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.2a1/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.2a1/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.2a1/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.2a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.2a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.2a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.2a1/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.2a1/reflex/py.typed
+-rw-r--r--   0        0        0    11041 2023-07-19 23:47:51.599199 reflex-0.2.2a1/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.2a1/reflex/route.py
+-rw-r--r--   0        0        0    31805 2023-07-14 23:13:37.781402 reflex-0.2.2a1/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.2a1/reflex/style.py
+-rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.2a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.2a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2023-07-20 20:03:35.350159 reflex-0.2.2a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.2a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     4225 2023-07-17 23:29:33.628283 reflex-0.2.2a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-07-14 23:13:37.782067 reflex-0.2.2a1/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-07-14 23:13:37.782125 reflex-0.2.2a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.2a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    14056 2023-07-19 01:58:26.541782 reflex-0.2.2a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     4105 2023-07-17 23:29:33.628618 reflex-0.2.2a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.2a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.2a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.2a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.2a1/reflex/vars.py
+-rw-r--r--   0        0        0     9586 1970-01-01 00:00:00.000000 reflex-0.2.2a1/PKG-INFO
```

### Comparing `reflex-0.2.1a2/LICENSE` & `reflex-0.2.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/README.md` & `reflex-0.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/pyproject.toml` & `reflex-0.2.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.1a2"
+version = "0.2.2a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.1a2/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.2a1/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/apps/default/default.py` & `reflex-0.2.2a1/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/assets/favicon.ico` & `reflex-0.2.2a1/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.2a1/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.2a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/web/bun.lockb` & `reflex-0.2.2a1/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/web/package.json` & `reflex-0.2.2a1/reflex/.templates/web/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'scripts'": "{'export-sitemap': 'next build && next-sitemap && next export -o _static'}"}*

```diff
@@ -36,10 +36,11 @@
         "postcss": "^8.4.24",
         "tailwindcss": "^3.3.2"
     },
     "name": "reflex",
     "scripts": {
         "dev": "next dev",
         "export": "next build && next export -o _static",
+        "export-sitemap": "next build && next-sitemap && next export -o _static",
         "prod": "next start"
     }
 }
```

### Comparing `reflex-0.2.1a2/reflex/.templates/web/pages/_app.js` & `reflex-0.2.2a1/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.2a1/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/.templates/web/utils/state.js` & `reflex-0.2.2a1/reflex/.templates/web/utils/state.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -227,16 +227,16 @@
         processing: true
     });
 
     // Apply the next event in the queue.
     const event = state.events.shift();
 
     // Set new events to avoid reprocessing the same event.
-    setState(state => ({
-        ...state,
+    setState(currentState => ({
+        ...currentState,
         events: state.events
     }));
 
     // Process events with handlers via REST and all others via websockets.
     let eventSent = false;
     if (event.handler) {
         eventSent = await applyRestEvent(event, state, setResult);
```

### Comparing `reflex-0.2.1a2/reflex/__init__.py` & `reflex-0.2.2a1/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/app.py` & `reflex-0.2.2a1/reflex/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,17 @@
 
     def __init__(self, *args, **kwargs):
         """Initialize the app.
 
         Args:
             *args: Args to initialize the app with.
             **kwargs: Kwargs to initialize the app with.
+
+        Raises:
+            ValueError: If the event namespace is not provided in the config.
         """
         super().__init__(*args, **kwargs)
 
         # Get the config
         config = get_config()
 
         # Add middleware.
@@ -124,17 +127,21 @@
             max_http_buffer_size=config.polling_max_http_buffer_size,
             ping_interval=constants.PING_INTERVAL,
             ping_timeout=constants.PING_TIMEOUT,
         )
 
         # Create the socket app. Note event endpoint constant replaces the default 'socket.io' path.
         self.socket_app = ASGIApp(self.sio, socketio_path="")
+        namespace = config.get_event_namespace()
+
+        if not namespace:
+            raise ValueError("event namespace must be provided in the config.")
 
         # Create the event namespace and attach the main app. Not related to any paths.
-        self.event_namespace = EventNamespace("/event", self)
+        self.event_namespace = EventNamespace(namespace, self)
 
         # Register the event namespace with the socket.
         self.sio.register_namespace(self.event_namespace)
         # Mount the socket app with the API.
         self.api.mount(str(constants.Endpoint.EVENT), self.socket_app)
 
         # Set up the admin dash.
```

### Comparing `reflex-0.2.1a2/reflex/base.py` & `reflex-0.2.2a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/compiler/compiler.py` & `reflex-0.2.2a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/compiler/templates.py` & `reflex-0.2.2a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/compiler/utils.py` & `reflex-0.2.2a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/__init__.py` & `reflex-0.2.2a1/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/base/bare.py` & `reflex-0.2.2a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/base/document.py` & `reflex-0.2.2a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/base/link.py` & `reflex-0.2.2a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/base/meta.py` & `reflex-0.2.2a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/base/script.py` & `reflex-0.2.2a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/component.py` & `reflex-0.2.2a1/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/code.py` & `reflex-0.2.2a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/datatable.py` & `reflex-0.2.2a1/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/divider.py` & `reflex-0.2.2a1/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/list.py` & `reflex-0.2.2a1/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/stat.py` & `reflex-0.2.2a1/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/table.py` & `reflex-0.2.2a1/reflex/components/datadisplay/table.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,15 +100,24 @@
             props: The properties of the component.
             rows (list[list], optional): The rows of the table body. Defaults to None.
 
         Returns:
             Component: _description_
         """
         if len(children) == 0:
-            children = [Tr.create(cell_type="data", cells=row) for row in rows or []]
+            if isinstance(rows, Var):
+                children = [
+                    Foreach.create(
+                        rows, lambda row: Tr.create(cell_type="data", cells=row)
+                    )
+                ]
+            else:
+                children = [
+                    Tr.create(cell_type="data", cells=row) for row in rows or []
+                ]
         return super().create(*children, **props)
 
 
 class Tfoot(ChakraComponent):
     """A table footer component."""
 
     tag = "Tfoot"
```

### Comparing `reflex-0.2.1a2/reflex/components/datadisplay/tag.py` & `reflex-0.2.2a1/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/disclosure/accordion.py` & `reflex-0.2.2a1/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/disclosure/tabs.py` & `reflex-0.2.2a1/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/disclosure/transition.py` & `reflex-0.2.2a1/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/feedback/alert.py` & `reflex-0.2.2a1/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/feedback/circularprogress.py` & `reflex-0.2.2a1/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/feedback/progress.py` & `reflex-0.2.2a1/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/feedback/skeleton.py` & `reflex-0.2.2a1/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/feedback/spinner.py` & `reflex-0.2.2a1/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/__init__.py` & `reflex-0.2.2a1/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/button.py` & `reflex-0.2.2a1/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/checkbox.py` & `reflex-0.2.2a1/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.2a1/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.2a1/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/debounce.py` & `reflex-0.2.2a1/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/editable.py` & `reflex-0.2.2a1/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/form.py` & `reflex-0.2.2a1/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/iconbutton.py` & `reflex-0.2.2a1/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/input.py` & `reflex-0.2.2a1/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/multiselect.py` & `reflex-0.2.2a1/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/numberinput.py` & `reflex-0.2.2a1/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/pininput.py` & `reflex-0.2.2a1/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/radio.py` & `reflex-0.2.2a1/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/rangeslider.py` & `reflex-0.2.2a1/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/select.py` & `reflex-0.2.2a1/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/slider.py` & `reflex-0.2.2a1/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/switch.py` & `reflex-0.2.2a1/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/textarea.py` & `reflex-0.2.2a1/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/forms/upload.py` & `reflex-0.2.2a1/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/graphing/plotly.py` & `reflex-0.2.2a1/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/graphing/victory.py` & `reflex-0.2.2a1/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/__init__.py` & `reflex-0.2.2a1/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/box.py` & `reflex-0.2.2a1/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/card.py` & `reflex-0.2.2a1/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/cond.py` & `reflex-0.2.2a1/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/flex.py` & `reflex-0.2.2a1/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/foreach.py` & `reflex-0.2.2a1/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/grid.py` & `reflex-0.2.2a1/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/html.py` & `reflex-0.2.2a1/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/responsive.py` & `reflex-0.2.2a1/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/stack.py` & `reflex-0.2.2a1/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/layout/wrap.py` & `reflex-0.2.2a1/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/libs/react_player.py` & `reflex-0.2.2a1/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/media/avatar.py` & `reflex-0.2.2a1/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/media/icon.py` & `reflex-0.2.2a1/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/media/image.py` & `reflex-0.2.2a1/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.2a1/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/navigation/link.py` & `reflex-0.2.2a1/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.2a1/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/navigation/stepper.py` & `reflex-0.2.2a1/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/__init__.py` & `reflex-0.2.2a1/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/alertdialog.py` & `reflex-0.2.2a1/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/banner.py` & `reflex-0.2.2a1/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/drawer.py` & `reflex-0.2.2a1/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/menu.py` & `reflex-0.2.2a1/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/modal.py` & `reflex-0.2.2a1/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/popover.py` & `reflex-0.2.2a1/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/overlay/tooltip.py` & `reflex-0.2.2a1/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/tags/iter_tag.py` & `reflex-0.2.2a1/reflex/components/tags/iter_tag.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tag to loop through a list of components."""
 from __future__ import annotations
 
 import inspect
 from typing import TYPE_CHECKING, Callable, List
 
 from reflex.components.tags.tag import Tag
-from reflex.vars import Var
+from reflex.vars import BaseVar, Var
 
 if TYPE_CHECKING:
     from reflex.components.component import Component
 
 
 INDEX_VAR = "i"
 
@@ -26,28 +26,31 @@
     @staticmethod
     def get_index_var() -> Var:
         """Get the index var for the tag.
 
         Returns:
             The index var.
         """
-        index = Var.create(INDEX_VAR, is_local=False)
-        assert index is not None
-        return index
+        return BaseVar(
+            name=INDEX_VAR,
+            type_=int,
+            is_local=True,
+        )
 
     @staticmethod
     def get_index_var_arg() -> Var:
         """Get the index var for the tag.
 
         Returns:
             The index var.
         """
-        arg = Var.create(INDEX_VAR)
-        assert arg is not None
-        return arg
+        return BaseVar(
+            name=INDEX_VAR,
+            type_=int,
+        )
 
     @staticmethod
     def render_component(render_fn: Callable, arg: Var) -> Component:
         """Render the component.
 
         Args:
             render_fn: The render function.
```

### Comparing `reflex-0.2.1a2/reflex/components/tags/tag.py` & `reflex-0.2.2a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/tags/tagless.py` & `reflex-0.2.2a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/typography/highlight.py` & `reflex-0.2.2a1/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/components/typography/markdown.py` & `reflex-0.2.2a1/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/config.py` & `reflex-0.2.2a1/reflex/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,14 +202,17 @@
 
     # Timeout when launching the gunicorn server.
     timeout: int = constants.TIMEOUT
 
     # Whether to enable or disable nextJS gzip compression.
     next_compression: bool = True
 
+    # The event namespace for ws connection
+    event_namespace: Optional[str] = constants.EVENT_NAMESPACE
+
     def __init__(self, *args, **kwargs):
         """Initialize the config values.
 
         If db_url is not provided gets it from db_config.
 
         Args:
             *args: The args to pass to the Pydantic init method.
@@ -247,14 +250,26 @@
             try:
                 if field.startswith("_"):
                     continue
                 setattr(self, field, getattr(constants, f"{field.upper()}"))
             except AttributeError:
                 pass
 
+    def get_event_namespace(self) -> Optional[str]:
+        """Get the websocket event namespace.
+
+        Returns:
+            The namespace for websocket.
+        """
+        if self.event_namespace:
+            return f'/{self.event_namespace.strip("/")}'
+
+        event_url = constants.Endpoint.EVENT.get_url()
+        return urllib.parse.urlsplit(event_url).path
+
 
 def get_config() -> Config:
     """Get the app config.
 
     Returns:
         The app config.
     """
```

### Comparing `reflex-0.2.1a2/reflex/constants.py` & `reflex-0.2.2a1/reflex/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,22 +65,24 @@
 JINJA_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "jinja")
 
 # The frontend directories in a project.
 # The web folder where the NextJS app is compiled to.
 WEB_DIR = ".web"
 # The name of the utils file.
 UTILS_DIR = "utils"
+# The name of the output static directory.
+STATIC_DIR = "_static"
 # The name of the state file.
 STATE_PATH = "/".join([UTILS_DIR, "state"])
 # The name of the components file.
 COMPONENTS_PATH = "/".join([UTILS_DIR, "components"])
 # The directory where the app pages are compiled to.
 WEB_PAGES_DIR = os.path.join(WEB_DIR, "pages")
 # The directory where the static build is located.
-WEB_STATIC_DIR = os.path.join(WEB_DIR, "_static")
+WEB_STATIC_DIR = os.path.join(WEB_DIR, STATIC_DIR)
 # The directory where the utils file is located.
 WEB_UTILS_DIR = os.path.join(WEB_DIR, UTILS_DIR)
 # The directory where the assets are located.
 WEB_ASSETS_DIR = os.path.join(WEB_DIR, "public")
 # The Tailwind config.
 TAILWIND_CONFIG = os.path.join(WEB_DIR, "tailwind.config.js")
 # Default Tailwind content paths
@@ -120,14 +122,16 @@
 TIMEOUT = get_value("TIMEOUT", 120, type_=int)
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
 # Socket.IO web server
 PING_INTERVAL = 25
 PING_TIMEOUT = 120
+# flag to make the engine print all the SQL statements it executes
+SQLALCHEMY_ECHO = get_value("SQLALCHEMY_ECHO", False, type_=bool)
 
 # Compiler variables.
 # The extension for compiled Javascript files.
 JS_EXT = ".js"
 # The extension for python files.
 PY_EXT = ".py"
 # The expected variable name where the rx.App is stored.
@@ -189,15 +193,16 @@
 CONFIG_FILE = f"{CONFIG_MODULE}{PY_EXT}"
 # The previous config file.
 OLD_CONFIG_FILE = f"pcconfig{PY_EXT}"
 # The deployment URL.
 PRODUCTION_BACKEND_URL = "https://{username}-{app_name}.api.pynecone.app"
 # Token expiration time in seconds.
 TOKEN_EXPIRATION = 60 * 60
-
+# The event namespace for websocket
+EVENT_NAMESPACE = get_value("EVENT_NAMESPACE")
 
 # Env modes
 class Env(str, Enum):
     """The environment modes."""
 
     DEV = "dev"
     PROD = "prod"
```

### Comparing `reflex-0.2.1a2/reflex/el/constants/html.py` & `reflex-0.2.2a1/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/el/constants/react.py` & `reflex-0.2.2a1/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/el/constants/reflex.py` & `reflex-0.2.2a1/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/el/element.py` & `reflex-0.2.2a1/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/el/elements/__init__.py` & `reflex-0.2.2a1/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/el/precompile.py` & `reflex-0.2.2a1/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/event.py` & `reflex-0.2.2a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.2a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/middleware/middleware.py` & `reflex-0.2.2a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/model.py` & `reflex-0.2.2a1/reflex/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,17 +36,20 @@
     url = url or conf.db_url
     if url is None:
         raise ValueError("No database url configured")
     if not Path(constants.ALEMBIC_CONFIG).exists():
         console.print(
             "[red]Database is not initialized, run [bold]reflex db init[/bold] first."
         )
+    echo_db_query = False
+    if conf.env == constants.Env.DEV and constants.SQLALCHEMY_ECHO:
+        echo_db_query = True
     return sqlmodel.create_engine(
         url,
-        echo=False,
+        echo=echo_db_query,
         connect_args={"check_same_thread": False} if conf.admin_dash else {},
     )
 
 
 class Model(Base, sqlmodel.SQLModel):
     """Base class to define a table in the database."""
```

### Comparing `reflex-0.2.1a2/reflex/reflex.py` & `reflex-0.2.2a1/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/route.py` & `reflex-0.2.2a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/state.py` & `reflex-0.2.2a1/reflex/state.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/style.py` & `reflex-0.2.2a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/testing.py` & `reflex-0.2.2a1/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/build.py` & `reflex-0.2.2a1/reflex/utils/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,23 +82,14 @@
         }
     )
 
     with open(constants.SITEMAP_CONFIG_FILE, "w") as f:
         f.write(templates.SITEMAP_CONFIG(config=config))
 
 
-def generate_sitemap():
-    """Generate the actual sitemap."""
-    subprocess.run(
-        [prerequisites.get_package_manager(), "run", "next-sitemap"],
-        cwd=constants.WEB_DIR,
-        stdout=subprocess.PIPE,
-    )
-
-
 def export_app(
     backend: bool = True,
     frontend: bool = True,
     zip: bool = False,
     deploy_url: Optional[str] = None,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
@@ -111,16 +102,18 @@
         deploy_url: The URL of the deployed app.
         loglevel: The log level to use.
     """
     # Remove the static folder.
     path_ops.rm(constants.WEB_STATIC_DIR)
 
     # Generate the sitemap file.
+    command = "export"
     if deploy_url is not None:
         generate_sitemap_config(deploy_url)
+        command = "export-sitemap"
 
     # Create a progress object
     progress = Progress(
         *Progress.get_default_columns()[:-1],
         MofNCompleteColumn(),
         TimeElapsedColumn(),
     )
@@ -139,15 +132,15 @@
 
     # Add a single task to the progress object
     task = progress.add_task("Creating Production Build: ", total=len(checkpoints))
 
     # Start the subprocess with the progress bar.
     try:
         with progress, new_process(
-            [prerequisites.get_package_manager(), "run", "export"],
+            [prerequisites.get_package_manager(), "run", command],
             cwd=constants.WEB_DIR,
         ) as export_process:
             assert export_process.stdout is not None, "No stdout for export process."
             for line in export_process.stdout:
                 if loglevel == constants.LogLevel.DEBUG:
                     print(line, end="")
 
@@ -164,18 +157,14 @@
     except Exception as e:
         console.print(f"[red]Export process errored: {e}")
         console.print(
             "[red]Run in with [bold]--loglevel debug[/bold] to see the full error."
         )
         os._exit(1)
 
-    # Generate the actual sitemap.
-    if deploy_url is not None:
-        generate_sitemap()
-
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
```

### Comparing `reflex-0.2.1a2/reflex/utils/console.py` & `reflex-0.2.2a1/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/exec.py` & `reflex-0.2.2a1/reflex/utils/exec.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/format.py` & `reflex-0.2.2a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/imports.py` & `reflex-0.2.2a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/path_ops.py` & `reflex-0.2.2a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/prerequisites.py` & `reflex-0.2.2a1/reflex/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/processes.py` & `reflex-0.2.2a1/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/telemetry.py` & `reflex-0.2.2a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/types.py` & `reflex-0.2.2a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/utils/watch.py` & `reflex-0.2.2a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/reflex/vars.py` & `reflex-0.2.2a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.1a2/PKG-INFO` & `reflex-0.2.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.1a2
+Version: 0.2.2a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

