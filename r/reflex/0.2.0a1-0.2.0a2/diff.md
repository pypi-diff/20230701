# Comparing `tmp/reflex-0.2.0a1.tar.gz` & `tmp/reflex-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.0a1.tar", max compression
+gzip compressed data, was "reflex-0.2.0a2.tar", max compression
```

## Comparing `reflex-0.2.0a1.tar` & `reflex-0.2.0a2.tar`

### file list

```diff
@@ -1,175 +1,175 @@
--rw-r--r--   0        0        0    11358 2023-06-27 19:44:11.125503 reflex-0.2.0a1/LICENSE
--rw-r--r--   0        0        0     8461 2023-06-27 19:44:11.125656 reflex-0.2.0a1/README.md
--rw-r--r--   0        0        0     1896 2023-06-28 21:02:04.387463 reflex-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-27 19:44:11.128524 reflex-0.2.0a1/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-06-27 19:44:11.128663 reflex-0.2.0a1/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-06-27 19:44:11.128732 reflex-0.2.0a1/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1226 2023-06-27 19:44:11.128954 reflex-0.2.0a1/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-06-27 19:44:11.129101 reflex-0.2.0a1/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-06-27 19:44:11.129299 reflex-0.2.0a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-06-27 19:44:11.129433 reflex-0.2.0a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-06-27 19:44:11.129488 reflex-0.2.0a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-06-27 19:44:11.129541 reflex-0.2.0a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-06-27 19:44:11.129632 reflex-0.2.0a1/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-06-27 19:44:11.129721 reflex-0.2.0a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-06-27 19:44:11.129809 reflex-0.2.0a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-06-27 19:44:11.129890 reflex-0.2.0a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-06-27 19:44:11.129970 reflex-0.2.0a1/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-06-27 19:44:11.130872 reflex-0.2.0a1/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-06-27 19:44:11.130961 reflex-0.2.0a1/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2023-06-27 19:44:11.131031 reflex-0.2.0a1/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1141 2023-06-27 19:44:11.131301 reflex-0.2.0a1/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-06-27 19:44:11.131463 reflex-0.2.0a1/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-06-27 19:44:11.131568 reflex-0.2.0a1/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-06-27 19:44:11.131644 reflex-0.2.0a1/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-06-27 19:44:11.131867 reflex-0.2.0a1/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-06-27 19:44:11.131951 reflex-0.2.0a1/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     9656 2023-06-28 21:01:51.884154 reflex-0.2.0a1/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1917 2023-06-28 21:01:51.884307 reflex-0.2.0a1/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-06-28 01:25:19.553569 reflex-0.2.0a1/reflex/admin.py
--rw-r--r--   0        0        0    22052 2023-06-28 01:25:19.553773 reflex-0.2.0a1/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-06-27 19:44:11.133013 reflex-0.2.0a1/reflex/base.py
--rw-r--r--   0        0        0       27 2023-06-27 19:44:11.133168 reflex-0.2.0a1/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     7367 2023-06-27 19:44:11.133323 reflex-0.2.0a1/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-06-27 19:44:11.133429 reflex-0.2.0a1/reflex/compiler/templates.py
--rw-r--r--   0        0        0     7751 2023-06-27 19:44:11.133957 reflex-0.2.0a1/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7471 2023-06-27 19:44:11.134065 reflex-0.2.0a1/reflex/components/__init__.py
--rw-r--r--   0        0        0      229 2023-06-27 19:44:11.134184 reflex-0.2.0a1/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-06-27 19:44:11.134368 reflex-0.2.0a1/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-06-27 19:44:11.134560 reflex-0.2.0a1/reflex/components/base/body.py
--rw-r--r--   0        0        0      721 2023-06-27 19:44:11.134715 reflex-0.2.0a1/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-06-27 19:44:11.134873 reflex-0.2.0a1/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-06-27 19:44:11.134990 reflex-0.2.0a1/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-06-27 19:44:11.135110 reflex-0.2.0a1/reflex/components/base/meta.py
--rw-r--r--   0        0        0    24223 2023-06-27 19:44:11.135393 reflex-0.2.0a1/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-06-27 19:44:11.135502 reflex-0.2.0a1/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-06-27 19:44:11.135630 reflex-0.2.0a1/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-06-27 19:44:11.135772 reflex-0.2.0a1/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     4025 2023-06-27 19:44:11.136022 reflex-0.2.0a1/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-06-27 19:44:11.136138 reflex-0.2.0a1/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-06-27 19:44:11.136281 reflex-0.2.0a1/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-06-27 19:44:11.136404 reflex-0.2.0a1/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-06-27 19:44:11.136541 reflex-0.2.0a1/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5785 2023-06-27 19:44:11.136687 reflex-0.2.0a1/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-06-27 19:44:11.136854 reflex-0.2.0a1/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-06-27 19:44:11.137000 reflex-0.2.0a1/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-06-27 19:44:11.137163 reflex-0.2.0a1/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-06-27 19:44:11.137730 reflex-0.2.0a1/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-06-27 19:44:11.137878 reflex-0.2.0a1/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-06-27 19:44:11.138089 reflex-0.2.0a1/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-06-27 19:44:11.138179 reflex-0.2.0a1/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1565 2023-06-27 19:44:11.138437 reflex-0.2.0a1/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-06-27 19:44:11.138584 reflex-0.2.0a1/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-06-27 19:44:11.138721 reflex-0.2.0a1/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-06-27 19:44:11.138852 reflex-0.2.0a1/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-06-27 19:44:11.138989 reflex-0.2.0a1/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1471 2023-06-27 19:44:11.139091 reflex-0.2.0a1/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-06-27 19:44:11.139232 reflex-0.2.0a1/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-06-27 19:44:11.139361 reflex-0.2.0a1/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-06-27 19:44:11.139608 reflex-0.2.0a1/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-06-27 19:44:11.139743 reflex-0.2.0a1/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-06-27 19:44:11.139887 reflex-0.2.0a1/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-06-27 19:44:11.140156 reflex-0.2.0a1/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1943 2023-06-27 19:44:11.140298 reflex-0.2.0a1/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-06-27 19:44:11.140427 reflex-0.2.0a1/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-06-27 19:44:11.140597 reflex-0.2.0a1/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-06-27 19:44:11.140858 reflex-0.2.0a1/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2872 2023-06-27 19:44:11.140996 reflex-0.2.0a1/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-06-27 19:44:11.141249 reflex-0.2.0a1/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-06-27 19:44:11.141372 reflex-0.2.0a1/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-06-27 19:44:11.141494 reflex-0.2.0a1/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-06-27 19:44:11.141620 reflex-0.2.0a1/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-06-27 19:44:11.141743 reflex-0.2.0a1/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-06-27 19:44:11.141920 reflex-0.2.0a1/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-06-27 19:44:11.142041 reflex-0.2.0a1/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-06-27 19:44:11.142160 reflex-0.2.0a1/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-06-27 19:44:11.142316 reflex-0.2.0a1/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-06-27 19:44:11.142445 reflex-0.2.0a1/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-06-27 19:44:11.142612 reflex-0.2.0a1/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-06-27 19:44:11.142690 reflex-0.2.0a1/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-06-27 19:44:11.142821 reflex-0.2.0a1/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-06-27 19:44:11.143107 reflex-0.2.0a1/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-06-27 19:44:11.143220 reflex-0.2.0a1/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-06-27 19:44:11.143353 reflex-0.2.0a1/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-06-27 19:44:11.143479 reflex-0.2.0a1/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-06-27 19:44:11.143617 reflex-0.2.0a1/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-06-27 19:44:11.143865 reflex-0.2.0a1/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-06-27 19:44:11.144010 reflex-0.2.0a1/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-06-27 19:44:11.144122 reflex-0.2.0a1/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-06-27 19:44:11.144331 reflex-0.2.0a1/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-06-27 19:44:11.144459 reflex-0.2.0a1/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-06-27 19:44:11.144576 reflex-0.2.0a1/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-06-27 19:44:11.144810 reflex-0.2.0a1/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-06-27 19:44:11.144963 reflex-0.2.0a1/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-06-27 19:44:11.145102 reflex-0.2.0a1/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-06-27 19:44:11.145217 reflex-0.2.0a1/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-06-27 19:44:11.145353 reflex-0.2.0a1/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-06-27 19:44:11.145602 reflex-0.2.0a1/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-06-27 19:44:11.145672 reflex-0.2.0a1/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-06-27 19:44:11.145809 reflex-0.2.0a1/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-06-27 19:44:11.145926 reflex-0.2.0a1/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-27 19:44:11.146020 reflex-0.2.0a1/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-06-27 19:44:11.146153 reflex-0.2.0a1/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-06-27 19:44:11.146292 reflex-0.2.0a1/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-06-27 19:44:11.146473 reflex-0.2.0a1/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-06-27 19:44:11.146591 reflex-0.2.0a1/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-06-27 19:44:11.146711 reflex-0.2.0a1/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-27 19:44:11.146794 reflex-0.2.0a1/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-06-27 19:44:11.146909 reflex-0.2.0a1/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1606 2023-06-27 19:44:11.147030 reflex-0.2.0a1/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-06-27 19:44:11.147151 reflex-0.2.0a1/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-06-27 19:44:11.147264 reflex-0.2.0a1/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-06-27 19:44:11.147387 reflex-0.2.0a1/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-27 19:44:11.147466 reflex-0.2.0a1/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-06-27 19:44:11.147600 reflex-0.2.0a1/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-06-27 19:44:11.147723 reflex-0.2.0a1/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-06-27 19:44:11.147856 reflex-0.2.0a1/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-06-27 19:44:11.147979 reflex-0.2.0a1/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-06-27 19:44:11.148109 reflex-0.2.0a1/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-06-27 19:44:11.148207 reflex-0.2.0a1/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-06-27 19:44:11.148335 reflex-0.2.0a1/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-06-27 19:44:11.148399 reflex-0.2.0a1/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-06-27 19:44:11.148512 reflex-0.2.0a1/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2294 2023-06-27 19:44:11.148635 reflex-0.2.0a1/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-06-27 19:44:11.148727 reflex-0.2.0a1/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-06-27 19:44:11.148966 reflex-0.2.0a1/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-06-27 19:44:11.149095 reflex-0.2.0a1/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-06-27 19:44:11.149223 reflex-0.2.0a1/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-06-27 19:44:11.149340 reflex-0.2.0a1/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3454 2023-06-27 19:44:11.149473 reflex-0.2.0a1/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-06-27 19:44:11.149590 reflex-0.2.0a1/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-06-27 19:44:11.149709 reflex-0.2.0a1/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7120 2023-06-27 19:44:11.149845 reflex-0.2.0a1/reflex/config.py
--rw-r--r--   0        0        0    10486 2023-06-27 19:44:11.149975 reflex-0.2.0a1/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-06-27 19:44:11.150039 reflex-0.2.0a1/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-06-27 19:44:11.150151 reflex-0.2.0a1/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-06-27 19:44:11.150219 reflex-0.2.0a1/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-06-27 19:44:11.150474 reflex-0.2.0a1/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-06-27 19:44:11.150571 reflex-0.2.0a1/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-06-27 19:44:11.150906 reflex-0.2.0a1/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-06-27 19:44:11.151244 reflex-0.2.0a1/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-06-27 19:44:11.151376 reflex-0.2.0a1/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-06-28 21:01:51.884492 reflex-0.2.0a1/reflex/event.py
--rw-r--r--   0        0        0      111 2023-06-27 19:44:11.151669 reflex-0.2.0a1/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-06-27 19:44:11.151870 reflex-0.2.0a1/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-06-27 19:44:11.151991 reflex-0.2.0a1/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     2382 2023-06-27 19:44:11.152120 reflex-0.2.0a1/reflex/model.py
--rw-r--r--   0        0        0        0 2023-06-27 19:44:11.152148 reflex-0.2.0a1/reflex/py.typed
--rw-r--r--   0        0        0     8891 2023-06-28 01:25:19.554153 reflex-0.2.0a1/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-06-27 19:44:11.152409 reflex-0.2.0a1/reflex/route.py
--rw-r--r--   0        0        0    31722 2023-06-28 01:25:19.554376 reflex-0.2.0a1/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-06-27 19:44:11.152777 reflex-0.2.0a1/reflex/style.py
--rw-r--r--   0        0        0       24 2023-06-27 19:44:11.152904 reflex-0.2.0a1/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7585 2023-06-28 01:25:15.379838 reflex-0.2.0a1/reflex/utils/build.py
--rw-r--r--   0        0        0     1759 2023-06-27 19:44:11.153226 reflex-0.2.0a1/reflex/utils/console.py
--rw-r--r--   0        0        0     4675 2023-06-28 01:25:15.380292 reflex-0.2.0a1/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-06-27 19:44:11.153473 reflex-0.2.0a1/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-06-27 19:44:11.153583 reflex-0.2.0a1/reflex/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-06-27 19:44:11.153645 reflex-0.2.0a1/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    12227 2023-06-27 19:44:11.153767 reflex-0.2.0a1/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     3734 2023-06-28 01:25:15.380501 reflex-0.2.0a1/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-06-27 19:44:11.154002 reflex-0.2.0a1/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-06-27 19:44:11.154115 reflex-0.2.0a1/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-06-27 19:44:11.154230 reflex-0.2.0a1/reflex/utils/watch.py
--rw-r--r--   0        0        0    31837 2023-06-27 19:44:11.154394 reflex-0.2.0a1/reflex/vars.py
--rw-r--r--   0        0        0    10138 1970-01-01 00:00:00.000000 reflex-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-27 19:44:11.125503 reflex-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0     8461 2023-06-27 19:44:11.125656 reflex-0.2.0a2/README.md
+-rw-r--r--   0        0        0     1896 2023-06-30 17:42:25.432387 reflex-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-27 19:44:11.128524 reflex-0.2.0a2/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-06-27 19:44:11.128663 reflex-0.2.0a2/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:44:11.128732 reflex-0.2.0a2/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1226 2023-06-27 19:44:11.128954 reflex-0.2.0a2/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-06-27 19:44:11.129101 reflex-0.2.0a2/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-06-27 19:44:11.129299 reflex-0.2.0a2/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-06-27 19:44:11.129433 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-06-27 19:44:11.129488 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-06-27 19:44:11.129541 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-27 19:44:11.129632 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-06-27 19:44:11.129721 reflex-0.2.0a2/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-06-27 19:44:11.129809 reflex-0.2.0a2/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-06-27 19:44:11.129890 reflex-0.2.0a2/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-06-27 19:44:11.129970 reflex-0.2.0a2/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-06-27 19:44:11.130872 reflex-0.2.0a2/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-06-27 19:44:11.130961 reflex-0.2.0a2/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2023-06-27 19:44:11.131031 reflex-0.2.0a2/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1141 2023-06-27 19:44:11.131301 reflex-0.2.0a2/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-06-27 19:44:11.131463 reflex-0.2.0a2/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-06-27 19:44:11.131568 reflex-0.2.0a2/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-06-27 19:44:11.131644 reflex-0.2.0a2/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-06-27 19:44:11.131867 reflex-0.2.0a2/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-06-27 19:44:11.131951 reflex-0.2.0a2/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     9656 2023-06-28 21:01:51.884154 reflex-0.2.0a2/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1917 2023-06-28 21:01:51.884307 reflex-0.2.0a2/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-06-28 01:25:19.553569 reflex-0.2.0a2/reflex/admin.py
+-rw-r--r--   0        0        0    22302 2023-06-30 17:42:07.289348 reflex-0.2.0a2/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-06-27 19:44:11.133013 reflex-0.2.0a2/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-06-27 19:44:11.133168 reflex-0.2.0a2/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     7404 2023-06-30 17:42:07.289532 reflex-0.2.0a2/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-06-27 19:44:11.133429 reflex-0.2.0a2/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8502 2023-06-30 17:42:07.289680 reflex-0.2.0a2/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7471 2023-06-27 19:44:11.134065 reflex-0.2.0a2/reflex/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-27 19:44:11.134184 reflex-0.2.0a2/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-27 19:44:11.134368 reflex-0.2.0a2/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-06-27 19:44:11.134560 reflex-0.2.0a2/reflex/components/base/body.py
+-rw-r--r--   0        0        0      721 2023-06-27 19:44:11.134715 reflex-0.2.0a2/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-06-27 19:44:11.134873 reflex-0.2.0a2/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-06-27 19:44:11.134990 reflex-0.2.0a2/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-06-27 19:44:11.135110 reflex-0.2.0a2/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    24223 2023-06-27 19:44:11.135393 reflex-0.2.0a2/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-06-27 19:44:11.135502 reflex-0.2.0a2/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-27 19:44:11.135630 reflex-0.2.0a2/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3518 2023-06-30 17:42:07.289969 reflex-0.2.0a2/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-06-27 19:44:11.136022 reflex-0.2.0a2/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-06-27 19:44:11.136138 reflex-0.2.0a2/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-06-27 19:44:11.136281 reflex-0.2.0a2/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-06-27 19:44:11.136404 reflex-0.2.0a2/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-06-27 19:44:11.136541 reflex-0.2.0a2/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5785 2023-06-27 19:44:11.136687 reflex-0.2.0a2/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-06-27 19:44:11.136854 reflex-0.2.0a2/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-06-27 19:44:11.137000 reflex-0.2.0a2/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-06-27 19:44:11.137163 reflex-0.2.0a2/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-06-27 19:44:11.137730 reflex-0.2.0a2/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-06-27 19:44:11.137878 reflex-0.2.0a2/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-06-27 19:44:11.138089 reflex-0.2.0a2/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-06-27 19:44:11.138179 reflex-0.2.0a2/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1565 2023-06-27 19:44:11.138437 reflex-0.2.0a2/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-06-27 19:44:11.138584 reflex-0.2.0a2/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-06-27 19:44:11.138721 reflex-0.2.0a2/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-06-27 19:44:11.138852 reflex-0.2.0a2/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-06-27 19:44:11.138989 reflex-0.2.0a2/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1471 2023-06-27 19:44:11.139091 reflex-0.2.0a2/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-06-27 19:44:11.139232 reflex-0.2.0a2/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-06-27 19:44:11.139361 reflex-0.2.0a2/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-06-27 19:44:11.139608 reflex-0.2.0a2/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-06-27 19:44:11.139743 reflex-0.2.0a2/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-06-27 19:44:11.139887 reflex-0.2.0a2/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-06-27 19:44:11.140156 reflex-0.2.0a2/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1943 2023-06-27 19:44:11.140298 reflex-0.2.0a2/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-06-27 19:44:11.140427 reflex-0.2.0a2/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-06-27 19:44:11.140597 reflex-0.2.0a2/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-06-27 19:44:11.140858 reflex-0.2.0a2/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2872 2023-06-27 19:44:11.140996 reflex-0.2.0a2/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-06-27 19:44:11.141249 reflex-0.2.0a2/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-06-27 19:44:11.141372 reflex-0.2.0a2/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-06-27 19:44:11.141494 reflex-0.2.0a2/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-06-27 19:44:11.141620 reflex-0.2.0a2/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-06-27 19:44:11.141743 reflex-0.2.0a2/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-06-27 19:44:11.141920 reflex-0.2.0a2/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-06-27 19:44:11.142041 reflex-0.2.0a2/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-06-27 19:44:11.142160 reflex-0.2.0a2/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-06-27 19:44:11.142316 reflex-0.2.0a2/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-06-27 19:44:11.142445 reflex-0.2.0a2/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-06-27 19:44:11.142612 reflex-0.2.0a2/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-06-27 19:44:11.142690 reflex-0.2.0a2/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-06-27 19:44:11.142821 reflex-0.2.0a2/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-06-27 19:44:11.143107 reflex-0.2.0a2/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-06-27 19:44:11.143220 reflex-0.2.0a2/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-27 19:44:11.143353 reflex-0.2.0a2/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-06-27 19:44:11.143479 reflex-0.2.0a2/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-06-27 19:44:11.143617 reflex-0.2.0a2/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-06-27 19:44:11.143865 reflex-0.2.0a2/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-06-27 19:44:11.144010 reflex-0.2.0a2/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-06-27 19:44:11.144122 reflex-0.2.0a2/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-06-27 19:44:11.144331 reflex-0.2.0a2/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-06-27 19:44:11.144459 reflex-0.2.0a2/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-06-27 19:44:11.144576 reflex-0.2.0a2/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-06-27 19:44:11.144810 reflex-0.2.0a2/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-06-27 19:44:11.144963 reflex-0.2.0a2/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-06-27 19:44:11.145102 reflex-0.2.0a2/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-06-27 19:44:11.145217 reflex-0.2.0a2/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-06-27 19:44:11.145353 reflex-0.2.0a2/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-06-27 19:44:11.145602 reflex-0.2.0a2/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-06-27 19:44:11.145672 reflex-0.2.0a2/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-27 19:44:11.145809 reflex-0.2.0a2/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-06-27 19:44:11.145926 reflex-0.2.0a2/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-27 19:44:11.146020 reflex-0.2.0a2/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-27 19:44:11.146153 reflex-0.2.0a2/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-06-27 19:44:11.146292 reflex-0.2.0a2/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-06-27 19:44:11.146473 reflex-0.2.0a2/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-06-27 19:44:11.146591 reflex-0.2.0a2/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-06-27 19:44:11.146711 reflex-0.2.0a2/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-27 19:44:11.146794 reflex-0.2.0a2/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-06-27 19:44:11.146909 reflex-0.2.0a2/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-06-30 17:42:07.290376 reflex-0.2.0a2/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-06-27 19:44:11.147151 reflex-0.2.0a2/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-06-27 19:44:11.147264 reflex-0.2.0a2/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-06-27 19:44:11.147387 reflex-0.2.0a2/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-27 19:44:11.147466 reflex-0.2.0a2/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-06-27 19:44:11.147600 reflex-0.2.0a2/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-06-27 19:44:11.147723 reflex-0.2.0a2/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-06-27 19:44:11.147856 reflex-0.2.0a2/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-06-27 19:44:11.147979 reflex-0.2.0a2/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-06-27 19:44:11.148109 reflex-0.2.0a2/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-06-27 19:44:11.148207 reflex-0.2.0a2/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-06-27 19:44:11.148335 reflex-0.2.0a2/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-06-27 19:44:11.148399 reflex-0.2.0a2/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-06-27 19:44:11.148512 reflex-0.2.0a2/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2294 2023-06-27 19:44:11.148635 reflex-0.2.0a2/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-06-27 19:44:11.148727 reflex-0.2.0a2/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-06-27 19:44:11.148966 reflex-0.2.0a2/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-06-27 19:44:11.149095 reflex-0.2.0a2/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-27 19:44:11.149223 reflex-0.2.0a2/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-06-27 19:44:11.149340 reflex-0.2.0a2/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3454 2023-06-27 19:44:11.149473 reflex-0.2.0a2/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-06-27 19:44:11.149590 reflex-0.2.0a2/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-06-27 19:44:11.149709 reflex-0.2.0a2/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7120 2023-06-27 19:44:11.149845 reflex-0.2.0a2/reflex/config.py
+-rw-r--r--   0        0        0    10486 2023-06-27 19:44:11.149975 reflex-0.2.0a2/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-06-27 19:44:11.150039 reflex-0.2.0a2/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-27 19:44:11.150151 reflex-0.2.0a2/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-06-27 19:44:11.150219 reflex-0.2.0a2/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-06-27 19:44:11.150474 reflex-0.2.0a2/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-06-27 19:44:11.150571 reflex-0.2.0a2/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-06-27 19:44:11.150906 reflex-0.2.0a2/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-06-27 19:44:11.151244 reflex-0.2.0a2/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-06-27 19:44:11.151376 reflex-0.2.0a2/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-06-28 21:01:51.884492 reflex-0.2.0a2/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-06-27 19:44:11.151669 reflex-0.2.0a2/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-06-27 19:44:11.151870 reflex-0.2.0a2/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-06-27 19:44:11.151991 reflex-0.2.0a2/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     2382 2023-06-27 19:44:11.152120 reflex-0.2.0a2/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-06-27 19:44:11.152148 reflex-0.2.0a2/reflex/py.typed
+-rw-r--r--   0        0        0     8891 2023-06-28 01:25:19.554153 reflex-0.2.0a2/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-06-27 19:44:11.152409 reflex-0.2.0a2/reflex/route.py
+-rw-r--r--   0        0        0    31805 2023-06-30 17:42:07.290862 reflex-0.2.0a2/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-06-27 19:44:11.152777 reflex-0.2.0a2/reflex/style.py
+-rw-r--r--   0        0        0       24 2023-06-27 19:44:11.152904 reflex-0.2.0a2/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7585 2023-06-28 01:25:15.379838 reflex-0.2.0a2/reflex/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-06-27 19:44:11.153226 reflex-0.2.0a2/reflex/utils/console.py
+-rw-r--r--   0        0        0     4680 2023-06-30 17:42:07.291282 reflex-0.2.0a2/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-06-30 17:42:02.061676 reflex-0.2.0a2/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-06-27 19:44:11.153583 reflex-0.2.0a2/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-06-30 17:42:07.291621 reflex-0.2.0a2/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    12296 2023-06-30 17:42:07.291811 reflex-0.2.0a2/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     3734 2023-06-28 23:03:00.473042 reflex-0.2.0a2/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-06-27 19:44:11.154002 reflex-0.2.0a2/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-06-27 19:44:11.154115 reflex-0.2.0a2/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-06-27 19:44:11.154230 reflex-0.2.0a2/reflex/utils/watch.py
+-rw-r--r--   0        0        0    31837 2023-06-27 19:44:11.154394 reflex-0.2.0a2/reflex/vars.py
+-rw-r--r--   0        0        0    10138 1970-01-01 00:00:00.000000 reflex-0.2.0a2/PKG-INFO
```

### Comparing `reflex-0.2.0a1/LICENSE` & `reflex-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/README.md` & `reflex-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/pyproject.toml` & `reflex-0.2.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.0a1/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.0a2/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/apps/default/default.py` & `reflex-0.2.0a2/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/assets/favicon.ico` & `reflex-0.2.0a2/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.0a2/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.0a2/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/web/bun.lockb` & `reflex-0.2.0a2/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/web/package.json` & `reflex-0.2.0a2/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/web/pages/_app.js` & `reflex-0.2.0a2/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.0a2/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/.templates/web/utils/state.js` & `reflex-0.2.0a2/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/__init__.py` & `reflex-0.2.0a2/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/app.py` & `reflex-0.2.0a2/reflex/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,30 +462,37 @@
             if config.tailwind is not None
             else {}
         )
 
         # Compile the pages.
         custom_components = set()
         thread_pool = ThreadPool()
+        compile_results = []
         for route, component in self.pages.items():
             component.add_style(self.style)
-            thread_pool.apply_async(
-                compiler.compile_page,
-                args=(
-                    route,
-                    component,
-                    self.state,
-                    self.connect_error_component,
-                ),
+            compile_results.append(
+                thread_pool.apply_async(
+                    compiler.compile_page,
+                    args=(
+                        route,
+                        component,
+                        self.state,
+                        self.connect_error_component,
+                    ),
+                )
             )
             # Add the custom components from the page to the set.
             custom_components |= component.get_custom_components()
         thread_pool.close()
         thread_pool.join()
 
+        # check the results of all the threads in case an exception was raised.
+        for r in compile_results:
+            r.get()
+
         # Compile the custom components.
         compiler.compile_components(custom_components)
 
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
 ) -> AsyncIterator[StateUpdate]:
```

### Comparing `reflex-0.2.0a1/reflex/base.py` & `reflex-0.2.0a2/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/compiler/compiler.py` & `reflex-0.2.0a2/reflex/compiler/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,19 +74,21 @@
     """Compile the component given the app state.
 
     Args:
         component: The component to compile.
         state: The app state.
         connect_error_component: The component to render on sever connection error.
 
+
     Returns:
         The compiled component.
     """
     # Merge the default imports with the app-specific imports.
     imports = utils.merge_imports(DEFAULT_IMPORTS, component.get_imports())
+    utils.validate_imports(imports)
     imports = utils.compile_imports(imports)
 
     # Compile the code to render the component.
     return templates.PAGE.render(
         imports=imports,
         custom_codes=component.get_custom_code(),
         initial_state=utils.compile_state(state),
```

### Comparing `reflex-0.2.0a1/reflex/compiler/templates.py` & `reflex-0.2.0a2/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/compiler/utils.py` & `reflex-0.2.0a2/reflex/compiler/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,36 @@
     # Get the default import, and the specific imports.
     default = next(iter({field.name for field in defaults}), "")
     rest = {field.name for field in fields - defaults}
 
     return default, rest
 
 
+def validate_imports(imports: imports.ImportDict):
+    """Verify that the same Tag is not used in multiple import.
+
+    Args:
+        imports: The dict of imports to validate
+
+    Raises:
+        ValueError: if a conflict on "tag/alias" is detected for an import.
+    """
+    used_tags = {}
+    for lib, _imports in imports.items():
+        for _import in _imports:
+            import_name = (
+                f"{_import.tag}/{_import.alias}" if _import.alias else _import.tag
+            )
+            if import_name in used_tags:
+                raise ValueError(
+                    f"Can not compile, the tag {import_name} is used multiple time from {lib} and {used_tags[import_name]}"
+                )
+            used_tags[import_name] = lib
+
+
 def compile_imports(imports: imports.ImportDict) -> List[dict]:
     """Compile an import dict.
 
     Args:
         imports: The import dict to compile.
 
     Returns:
```

### Comparing `reflex-0.2.0a1/reflex/components/__init__.py` & `reflex-0.2.0a2/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/base/bare.py` & `reflex-0.2.0a2/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/base/document.py` & `reflex-0.2.0a2/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/base/link.py` & `reflex-0.2.0a2/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/base/meta.py` & `reflex-0.2.0a2/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/component.py` & `reflex-0.2.0a2/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/code.py` & `reflex-0.2.0a2/reflex/components/datadisplay/code.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 
     # A custom style for the code block.
     custom_style: Var[Dict[str, str]]
 
     # Props passed down to the code tag.
     code_tag_props: Var[Dict[str, str]]
 
+    is_default = True
+
     def _get_imports(self) -> imports.ImportDict:
         merged_imports = super()._get_imports()
         if self.theme is not None:
             merged_imports = imports.merge_imports(
                 merged_imports, {PRISM_STYLES_PATH: {ImportVar(tag=self.theme.name)}}
             )
         return merged_imports
```

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/datatable.py` & `reflex-0.2.0a2/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/divider.py` & `reflex-0.2.0a2/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/list.py` & `reflex-0.2.0a2/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/stat.py` & `reflex-0.2.0a2/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/table.py` & `reflex-0.2.0a2/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/datadisplay/tag.py` & `reflex-0.2.0a2/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/disclosure/accordion.py` & `reflex-0.2.0a2/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/disclosure/tabs.py` & `reflex-0.2.0a2/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/disclosure/transition.py` & `reflex-0.2.0a2/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/feedback/alert.py` & `reflex-0.2.0a2/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/feedback/circularprogress.py` & `reflex-0.2.0a2/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/feedback/progress.py` & `reflex-0.2.0a2/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/feedback/skeleton.py` & `reflex-0.2.0a2/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/feedback/spinner.py` & `reflex-0.2.0a2/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/__init__.py` & `reflex-0.2.0a2/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/button.py` & `reflex-0.2.0a2/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/checkbox.py` & `reflex-0.2.0a2/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.0a2/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.0a2/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/editable.py` & `reflex-0.2.0a2/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/form.py` & `reflex-0.2.0a2/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/iconbutton.py` & `reflex-0.2.0a2/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/input.py` & `reflex-0.2.0a2/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/multiselect.py` & `reflex-0.2.0a2/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/numberinput.py` & `reflex-0.2.0a2/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/pininput.py` & `reflex-0.2.0a2/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/radio.py` & `reflex-0.2.0a2/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/rangeslider.py` & `reflex-0.2.0a2/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/select.py` & `reflex-0.2.0a2/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/slider.py` & `reflex-0.2.0a2/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/switch.py` & `reflex-0.2.0a2/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/textarea.py` & `reflex-0.2.0a2/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/forms/upload.py` & `reflex-0.2.0a2/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/graphing/plotly.py` & `reflex-0.2.0a2/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/graphing/victory.py` & `reflex-0.2.0a2/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/__init__.py` & `reflex-0.2.0a2/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/box.py` & `reflex-0.2.0a2/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/card.py` & `reflex-0.2.0a2/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/cond.py` & `reflex-0.2.0a2/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/flex.py` & `reflex-0.2.0a2/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/foreach.py` & `reflex-0.2.0a2/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/grid.py` & `reflex-0.2.0a2/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/html.py` & `reflex-0.2.0a2/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/responsive.py` & `reflex-0.2.0a2/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/stack.py` & `reflex-0.2.0a2/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/layout/wrap.py` & `reflex-0.2.0a2/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/libs/react_player.py` & `reflex-0.2.0a2/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/media/avatar.py` & `reflex-0.2.0a2/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/media/icon.py` & `reflex-0.2.0a2/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/media/image.py` & `reflex-0.2.0a2/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.0a2/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/navigation/link.py` & `reflex-0.2.0a2/reflex/components/navigation/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,11 +47,11 @@
         Returns:
             Component: The link component
         """
         if href and not len(children):
             raise ValueError("Link without a child will not display")
         elif href is None and len(children):
             # Don't use a NextLink if there is no href.
-            props["as_"] = "Link"
+            props["as_"] = ""
         if href:
             props["href"] = href
         return super().create(*children, **props)
```

### Comparing `reflex-0.2.0a1/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.0a2/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/navigation/stepper.py` & `reflex-0.2.0a2/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/__init__.py` & `reflex-0.2.0a2/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/alertdialog.py` & `reflex-0.2.0a2/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/banner.py` & `reflex-0.2.0a2/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/drawer.py` & `reflex-0.2.0a2/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/menu.py` & `reflex-0.2.0a2/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/modal.py` & `reflex-0.2.0a2/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/popover.py` & `reflex-0.2.0a2/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/overlay/tooltip.py` & `reflex-0.2.0a2/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/tags/iter_tag.py` & `reflex-0.2.0a2/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/tags/tag.py` & `reflex-0.2.0a2/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/tags/tagless.py` & `reflex-0.2.0a2/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/typography/highlight.py` & `reflex-0.2.0a2/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/components/typography/markdown.py` & `reflex-0.2.0a2/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/config.py` & `reflex-0.2.0a2/reflex/config.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/constants.py` & `reflex-0.2.0a2/reflex/constants.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/el/constants/html.py` & `reflex-0.2.0a2/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/el/constants/react.py` & `reflex-0.2.0a2/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/el/constants/reflex.py` & `reflex-0.2.0a2/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/el/element.py` & `reflex-0.2.0a2/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/el/elements/__init__.py` & `reflex-0.2.0a2/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/el/precompile.py` & `reflex-0.2.0a2/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/event.py` & `reflex-0.2.0a2/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.0a2/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/middleware/middleware.py` & `reflex-0.2.0a2/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/model.py` & `reflex-0.2.0a2/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/reflex.py` & `reflex-0.2.0a2/reflex/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/route.py` & `reflex-0.2.0a2/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/state.py` & `reflex-0.2.0a2/reflex/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import functools
 import inspect
 import json
 import traceback
 import urllib.parse
 from abc import ABC
 from collections import defaultdict
+from types import FunctionType
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     ClassVar,
     Dict,
     List,
@@ -193,14 +194,15 @@
             cls.inherited_backend_vars = parent_state.backend_vars
 
         cls.new_backend_vars = {
             name: value
             for name, value in cls.__dict__.items()
             if types.is_backend_variable(name)
             and name not in cls.inherited_backend_vars
+            and not isinstance(value, FunctionType)
         }
 
         cls.backend_vars = {**cls.inherited_backend_vars, **cls.new_backend_vars}
 
         # Set the base and computed vars.
         cls.base_vars = {
             f.name: BaseVar(name=f.name, type_=f.outer_type_).set_state(cls)
```

### Comparing `reflex-0.2.0a1/reflex/style.py` & `reflex-0.2.0a2/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/build.py` & `reflex-0.2.0a2/reflex/utils/build.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/console.py` & `reflex-0.2.0a2/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/exec.py` & `reflex-0.2.0a2/reflex/utils/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         str(port),
         "--log-level",
         loglevel,
         "--reload",
         "--reload-exclude",
         f"'{constants.WEB_DIR}/*'",
     ]
-    process = new_process(cmd)
+    process = subprocess.Popen(cmd)
 
     try:
         process.wait()
     except KeyboardInterrupt:
         process.terminate()
```

### Comparing `reflex-0.2.0a1/reflex/utils/format.py` & `reflex-0.2.0a2/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/imports.py` & `reflex-0.2.0a2/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/path_ops.py` & `reflex-0.2.0a2/reflex/utils/path_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,15 @@
 
 def mkdir(path: str):
     """Create a directory.
 
     Args:
         path: The path to the directory.
     """
-    if not os.path.exists(path):
-        os.makedirs(path)
+    os.makedirs(path, exist_ok=True)
 
 
 def ln(src: str, dest: str, overwrite: bool = False) -> bool:
     """Create a symbolic link.
 
     Args:
         src: The path to the file or directory.
```

### Comparing `reflex-0.2.0a1/reflex/utils/prerequisites.py` & `reflex-0.2.0a2/reflex/utils/prerequisites.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,16 +384,18 @@
     # Add the config file to the list of files to be migrated.
     file_list.append(constants.CONFIG_FILE)
 
     # Migrate all files.
     updates = {
         "Pynecone": "Reflex",
         "pynecone as pc": "reflex as rx",
+        "pynecone.io": "reflex.dev",
         "pynecone": "reflex",
         "pc.": "rx.",
+        "pcconfig": "rxconfig",
     }
     for file_path in file_list:
         with FileInput(file_path, inplace=True) as file:
             for line in file:
                 for old, new in updates.items():
                     line = line.replace(old, new)
                 print(line, end="")
```

### Comparing `reflex-0.2.0a1/reflex/utils/processes.py` & `reflex-0.2.0a2/reflex/utils/processes.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/telemetry.py` & `reflex-0.2.0a2/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/types.py` & `reflex-0.2.0a2/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/utils/watch.py` & `reflex-0.2.0a2/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/reflex/vars.py` & `reflex-0.2.0a2/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.0a1/PKG-INFO` & `reflex-0.2.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

