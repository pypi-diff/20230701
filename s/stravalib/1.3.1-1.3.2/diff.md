# Comparing `tmp/stravalib-1.3.1.tar.gz` & `tmp/stravalib-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stravalib-1.3.1.tar", last modified: Fri Jun 16 17:48:19 2023, max compression
+gzip compressed data, was "stravalib-1.3.2.tar", last modified: Sat Jul  1 08:08:46 2023, max compression
```

## Comparing `stravalib-1.3.1.tar` & `stravalib-1.3.2.tar`

### file list

```diff
@@ -1,190 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.723691 stravalib-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 17:48:00.000000 stravalib-1.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-16 17:48:00.000000 stravalib-1.3.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.691691 stravalib-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.691691 stravalib-1.3.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-16 17:48:00.000000 stravalib-1.3.1/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-16 17:48:00.000000 stravalib-1.3.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.691691 stravalib-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-16 17:48:00.000000 stravalib-1.3.1/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-16 17:48:00.000000 stravalib-1.3.1/.github/workflows/build-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-16 17:48:00.000000 stravalib-1.3.1/.github/workflows/check-strava-api.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-16 17:48:00.000000 stravalib-1.3.1/.github/workflows/push-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 17:48:00.000000 stravalib-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-16 17:48:00.000000 stravalib-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 17:48:00.000000 stravalib-1.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-06-16 17:48:00.000000 stravalib-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-16 17:48:00.000000 stravalib-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 17:48:00.000000 stravalib-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-16 17:48:00.000000 stravalib-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-16 17:48:00.000000 stravalib-1.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-16 17:48:19.723691 stravalib-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-16 17:48:00.000000 stravalib-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-16 17:48:00.000000 stravalib-1.3.1/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.691691 stravalib-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.691691 stravalib-1.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/_static/keepme
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/_static/stravalib.css
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.691691 stravalib-1.3.1/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/contributing/build-release-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/contributing/development-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/contributing/documentation-changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/contributing/how-to-contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/contributing/resources-for-new-contributors.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.695691 stravalib-1.3.1/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/get-started/activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/get-started/athletes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/get-started/authenticate-with-strava.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/get-started/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/get-started/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.695691 stravalib-1.3.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/images/stravalib_architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.695691 stravalib-1.3.1/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.711691 stravalib-1.3.1/docs/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.ActivityUploader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.ActivityUploader.update_from_response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.BatchedResultsIterator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.authorization_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.create_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.create_subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.deauthorize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.delete_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.delete_subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.exchange_code_for_token.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.explore_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity_comments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity_kudos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity_laps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity_photos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_activity_zones.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_athlete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_athlete_clubs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_athlete_koms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_athlete_starred_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_athlete_stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_club_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_club_members.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_effort_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_friend_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_gear.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_related_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_route_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_routes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_segment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_segment_effort.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_segment_efforts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_segment_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.get_starred_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.handle_subscription_callback.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.handle_subscription_update.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.join_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.leave_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.list_subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.refresh_access_token.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.update_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.update_athlete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.client.Client.upload_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.field_conversions.enum_value.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.field_conversions.enum_values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.field_conversions.optional_input.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.field_conversions.time_interval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.field_conversions.timezone.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.unithelper.Quantity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.unithelper.UnitConverter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.unithelper.c2f.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.unithelper.is_quantity_type.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.RateLimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/api/stravalib.util.limiter.total_seconds.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/field-conversions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/strava_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/unithelper.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 17:48:00.000000 stravalib-1.3.1/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 17:48:00.000000 stravalib-1.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.683691 stravalib-1.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.711691 stravalib-1.3.1/examples/strava-oauth/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.711691 stravalib-1.3.1/examples/strava-oauth/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/static/ConnectWithStrava.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.711691 stravalib-1.3.1/examples/strava-oauth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/templates/login_error.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 17:48:00.000000 stravalib-1.3.1/examples/strava-oauth/templates/login_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-16 17:48:00.000000 stravalib-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 17:48:00.000000 stravalib-1.3.1/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 17:48:00.000000 stravalib-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:48:19.723691 stravalib-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.715691 stravalib-1.3.1/stravalib/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 17:48:19.000000 stravalib-1.3.1/stravalib/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    69645 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    36042 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/strava_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.715691 stravalib-1.3.1/stravalib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/auth_responder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.715691 stravalib-1.3.1/stravalib/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/functional/test_client_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/functional/test_client_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/functional/test_result_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.715691 stravalib-1.3.1/stravalib/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/integration/strava_api_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)    24592 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/integration/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.719691 stravalib-1.3.1/stravalib/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/activity-manual.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/activity.3.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/athlete.2.json
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/athlete.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/example_route_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/example_zone_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   451575 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/sample.tcx
--rw-r--r--   0 runner    (1001) docker     (123)   102646 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/resources/strava_swagger.json
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/test.ini-example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.719691 stravalib-1.3.1/stravalib/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/unit/test_client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/unit/test_field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/unit/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/tests/unit/test_unithelper.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/unit_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/unithelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.723691 stravalib-1.3.1/stravalib/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-06-16 17:48:00.000000 stravalib-1.3.1/stravalib/util/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:48:19.715691 stravalib-1.3.1/stravalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-16 17:48:19.000000 stravalib-1.3.1/stravalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-06-16 17:48:19.000000 stravalib-1.3.1/stravalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:48:19.000000 stravalib-1.3.1/stravalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 17:48:19.000000 stravalib-1.3.1/stravalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-16 17:48:19.000000 stravalib-1.3.1/stravalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 08:08:30.000000 stravalib-1.3.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-01 08:08:30.000000 stravalib-1.3.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/build-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/check-strava-api.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/push-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/type-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-01 08:08:30.000000 stravalib-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-01 08:08:30.000000 stravalib-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 08:08:30.000000 stravalib-1.3.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-01 08:08:30.000000 stravalib-1.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-01 08:08:30.000000 stravalib-1.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-01 08:08:30.000000 stravalib-1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 08:08:30.000000 stravalib-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-01 08:08:30.000000 stravalib-1.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-01 08:08:46.844701 stravalib-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-01 08:08:30.000000 stravalib-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-01 08:08:30.000000 stravalib-1.3.2/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/_static/keepme
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/_static/stravalib.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/build-release-guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/development-guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/documentation-changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/how-to-contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/resources-for-new-contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/athletes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/authenticate-with-strava.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/images/stravalib_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/docs/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.ActivityUploader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.ActivityUploader.update_from_response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.BatchedResultsIterator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.authorization_url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.create_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.create_subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.deauthorize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.delete_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.delete_subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.exchange_code_for_token.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.explore_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_comments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_kudos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_laps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_photos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_zones.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_clubs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_koms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_starred_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_club_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_club_members.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_effort_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_friend_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_gear.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_related_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_route_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_routes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment_effort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment_efforts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_starred_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.handle_subscription_callback.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.handle_subscription_update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.join_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.leave_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.list_subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.refresh_access_token.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.update_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.update_athlete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.upload_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.enum_value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.enum_values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.optional_input.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.time_interval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.timezone.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.Quantity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.UnitConverter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.c2f.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.is_quantity_type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.LimitStructure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.LimitsStructure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.RateLimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.RequestRate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/field-conversions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/strava_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/unithelper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 08:08:30.000000 stravalib-1.3.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/examples/strava-oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/examples/strava-oauth/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/static/ConnectWithStrava.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/examples/strava-oauth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/templates/login_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/templates/login_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 08:08:30.000000 stravalib-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-01 08:08:30.000000 stravalib-1.3.2/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 08:08:30.000000 stravalib-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:08:46.844701 stravalib-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib/_version_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69653 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36042 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/strava_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/auth_responder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_client_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_client_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_result_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/strava_api_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24592 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/stravalib/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/activity-manual.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/activity.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/athlete.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/athlete.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/example_route_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/example_zone_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   451575 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/sample.tcx
+-rw-r--r--   0 runner    (1001) docker     (123)   102646 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/strava_swagger.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/test.ini-example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/stravalib/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_unithelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/unit_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/unithelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/stravalib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/util/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/top_level.txt
```

### Comparing `stravalib-1.3.1/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md` & `stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/.github/PULL_REQUEST_TEMPLATE.md` & `stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/.github/workflows/build-docs.yml` & `stravalib-1.3.2/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/.github/workflows/build-test.yml` & `stravalib-1.3.2/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/.github/workflows/check-strava-api.yml` & `stravalib-1.3.2/.github/workflows/check-strava-api.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/.github/workflows/push-pypi.yml` & `stravalib-1.3.2/.github/workflows/push-pypi.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/.pre-commit-config.yaml` & `stravalib-1.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/CODE_OF_CONDUCT.md` & `stravalib-1.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/CONTRIBUTING.md` & `stravalib-1.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/LICENSE.txt` & `stravalib-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/Makefile` & `stravalib-1.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/PKG-INFO` & `stravalib-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stravalib
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
 Author-email: Hans Lellelid <hans@xmpl.org>
 Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong
 License: Apache 2.0 License
 Project-URL: homepage, https://example.com
 Project-URL: documentation, https://stravalib.readthedocs.io
 Project-URL: repository, https://github.com/stravalib/stravalib
```

### Comparing `stravalib-1.3.1/README.md` & `stravalib-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/changelog.md` & `stravalib-1.3.2/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # Change Log
 
 ## Unreleased
 
+## v1.3.2
+
+### Added
+
+- Add: type checking to limiter, protocol and exc file (@enadeau , #374)
+
+### Fixed
+
+- Fix: two minor mistakes in documentation (@enadeau , #375)
+- Fix: pins pydantic to v1 (@lwasser, #380)
+
+### Contributors to this release
+
+@enadeau, @lwasser
+
 ## v1.3.1
 
 ### Added
 
 - Add: Add field override in class Segment to support all activity types (@solorisx, #368)
 
 ### Fixed
```

### Comparing `stravalib-1.3.1/docs/Makefile` & `stravalib-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/conf.py` & `stravalib-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/contributing/build-release-guide.md` & `stravalib-1.3.2/docs/contributing/build-release-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/contributing/development-guide.md` & `stravalib-1.3.2/docs/contributing/development-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/contributing/resources-for-new-contributors.md` & `stravalib-1.3.2/docs/contributing/resources-for-new-contributors.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/get-started/activities.rst` & `stravalib-1.3.2/docs/get-started/activities.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/get-started/athletes.rst` & `stravalib-1.3.2/docs/get-started/athletes.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/get-started/authenticate-with-strava.rst` & `stravalib-1.3.2/docs/get-started/authenticate-with-strava.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/get-started/index.md` & `stravalib-1.3.2/docs/get-started/index.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/get-started/overview.rst` & `stravalib-1.3.2/docs/get-started/overview.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/images/stravalib_architecture.png` & `stravalib-1.3.2/docs/images/stravalib_architecture.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/index.md` & `stravalib-1.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/reference/api/stravalib.client.ActivityUploader.rst` & `stravalib-1.3.2/docs/reference/api/stravalib.client.ActivityUploader.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/reference/api/stravalib.client.Client.rst` & `stravalib-1.3.2/docs/reference/api/stravalib.client.Client.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/reference/client.rst` & `stravalib-1.3.2/docs/reference/client.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/reference/model.rst` & `stravalib-1.3.2/docs/reference/model.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/docs/reference/utilities.rst` & `stravalib-1.3.2/docs/reference/utilities.rst`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 Limiter - in Utility Submodule: Functions and Classes
 ======================================================
 .. currentmodule:: stravalib.util.limiter
 
 This module provides a mixture of helpers to support rate limiting
 and also functions for conversion?
 
-**TODO:** look into whether total_seconds relates to limiter actions or
-unit conversion
-
 Summary Functions
 -------------------------------
 .. autosummary::
    :toctree: api/
 
-   total_seconds
    get_rates_from_response_headers
    get_seconds_until_next_quarter
    get_seconds_until_next_day
 
 
 Summary Classes
 -------------------------------
@@ -26,7 +22,10 @@
    :toctree: api/
 
    XRateLimitRule
    SleepingRateLimitRule
    RateLimitRule
    RateLimiter
    DefaultRateLimiter
+   RequestRate
+   LimitStructure
+   LimitsStructure
```

### Comparing `stravalib-1.3.1/docs/reference.rst` & `stravalib-1.3.2/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/examples/strava-oauth/README.md` & `stravalib-1.3.2/examples/strava-oauth/README.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/examples/strava-oauth/server.py` & `stravalib-1.3.2/examples/strava-oauth/server.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/examples/strava-oauth/static/ConnectWithStrava.png` & `stravalib-1.3.2/examples/strava-oauth/static/ConnectWithStrava.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/examples/strava-oauth/templates/login.html` & `stravalib-1.3.2/examples/strava-oauth/templates/login.html`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/pyproject.toml` & `stravalib-1.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -69,7 +69,34 @@
 profile = "black"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::FutureWarning:stravalib.*",
     "ignore::DeprecationWarning:stravalib.*"
 ]
+
+[tool.mypy]
+python_version = "3.8"
+follow_imports = "silent"
+warn_redundant_casts = true
+warn_unused_ignores = true
+disallow_any_generics = true
+check_untyped_defs = true
+no_implicit_reexport = true
+warn_unreachable = true
+disallow_untyped_defs = true
+
+plugins = [
+  "pydantic.mypy"
+]
+
+files = [
+    "stravalib/util/limiter.py",
+    "stravalib/protocol.py",
+    "stravalib/exc.py",
+]
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
```

### Comparing `stravalib-1.3.1/stravalib/client.py` & `stravalib-1.3.2/stravalib/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -832,16 +832,16 @@
             WARNING - This param is supported (as of 2022-11-15), but not
             documented and may be removed in the future.
         private : bool, optional, default=None
             Set to True to mark the resulting activity as private,
             'view_private' permissions will be necessary to view the activity.
 
             .. deprecated:: 1.0
-            This param is not supported by the Strava API and may be
-            removed in the future.
+                This param is not supported by the Strava API and may be
+                removed in the future.
         external_id : str, optional, default=None
             An arbitrary unique identifier may be specified which
             will be included in status responses.
         trainer : bool, optional, default=None
             Whether the resulting activity should be marked as having
             been performed on a trainer.
         commute : bool, optional, default=None
```

### Comparing `stravalib-1.3.1/stravalib/exc.py` & `stravalib-1.3.2/stravalib/exc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Exceptions & Error Handling
 ============================
 Exceptions and error handling for stravalib.
 These are classes designed to capture and handle various errors encountered when interacting with the Strava API.
 """
+from __future__ import annotations
+
 import logging
 import warnings
-from typing import Type
 
 import requests.exceptions
 
 
 class AuthError(RuntimeError):
     pass
 
@@ -52,16 +53,21 @@
 class RateLimitExceeded(RuntimeError):
     """
     Exception raised when the client rate limit has been exceeded.
 
     https://developers.strava.com/docs/rate-limits/
     """
 
-    def __init__(self, msg, timeout=None, limit=None):
-        super(RateLimitExceeded, self).__init__()
+    def __init__(
+        self,
+        msg: str,
+        timeout: float | None = None,
+        limit: float | None = None,
+    ) -> None:
+        super().__init__()
         self.limit = limit
         self.timeout = timeout
 
 
 class RateLimitTimeout(RateLimitExceeded):
     """
     Exception raised when the client rate limit has been exceeded
@@ -105,78 +111,81 @@
 
 # Warnings configuration and helper functions
 warnings.simplefilter("default")
 logging.captureWarnings(True)
 
 
 def warn_method_deprecation(
-    klass: Type, method_name: str, alternative: str, alt_url: str = None
-):
+    klass: type,
+    method_name: str,
+    alternative: str,
+    alt_url: str | None = None,
+) -> None:
     alt_support_msg = (
         f" See {alt_url} for more information." if alt_url else ""
     )
     warnings.warn(
         f'The method "{method_name}" of class "{klass}" is deprecated and will be '
         f'removed in the future. Instead, you can use "{alternative}".{alt_support_msg}',
         DeprecationWarning,
         stacklevel=3,
     )
 
 
-def warn_param_unsupported(param_name: str):
+def warn_param_unsupported(param_name: str) -> None:
     warnings.warn(
         f'The "{param_name}" parameter is unsupported by the Strava API. It has no '
         "effect and may lead to errors in the future.",
         DeprecationWarning,
         stacklevel=3,
     )
 
 
 def warn_param_deprecation(
-    param_name: str, alternative: str, alt_url: str = None
-):
+    param_name: str, alternative: str, alt_url: str | None = None
+) -> None:
     alt_support_msg = (
         f" See {alt_url} for more information." if alt_url else ""
     )
     warnings.warn(
         f'The "{param_name}" parameter is deprecated and will be removed'
         f'in the future. Instead, you can use "{alternative}".{alt_support_msg}',
         DeprecationWarning,
         stacklevel=3,
     )
 
 
-def warn_param_unofficial(param_name: str):
+def warn_param_unofficial(param_name: str) -> None:
     warnings.warn(
         f'The "{param_name}" parameter is undocumented in the Strava API. Its use '
         "may lead to unexpected behavior or errors in the future.",
         FutureWarning,
         stacklevel=3,
     )
 
 
-def warn_attribute_unofficial(attr_name: str):
+def warn_attribute_unofficial(attr_name: str) -> None:
     warnings.warn(
         f'The "{attr_name}" parameter is undocumented in the Strava API. Its use '
         "may lead to unexpected behavior or errors in the future.",
         FutureWarning,
         stacklevel=3,
     )
 
 
-def warn_method_unofficial(method_name: str):
+def warn_method_unofficial(method_name: str) -> None:
     warnings.warn(
         f'The "{method_name}" method is undocumented in the Strava API. Its use '
         "may lead to unexpected behavior or errors in the future.",
         FutureWarning,
         stacklevel=3,
     )
 
 
-def warn_units_deprecated():
+def warn_units_deprecated() -> None:
     warnings.warn(
         "You are using a Quantity object or attributes from the units library, which is "
         "deprecated. Support for these types will be removed in the future. Instead, "
         "please use Quantity objects from the Pint package (https://pint.readthedocs.io).",
         DeprecationWarning,
         stacklevel=3,
     )
```

### Comparing `stravalib-1.3.1/stravalib/field_conversions.py` & `stravalib-1.3.2/stravalib/field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/model.py` & `stravalib-1.3.2/stravalib/model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/protocol.py` & `stravalib-1.3.2/stravalib/protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,68 @@
 """
 Protocol
 ==============
 Low-level classes for interacting directly with the Strava API webservers.
 """
+from __future__ import annotations
+
 import abc
 import functools
 import logging
+from typing import TYPE_CHECKING, Any, Callable, Literal, TypedDict
 from urllib.parse import urlencode, urljoin, urlunsplit
 
 import requests
 
 from stravalib import exc
 
+if TYPE_CHECKING:
+    from _typeshed import SupportsRead
+
+Scope = Literal[
+    "read",
+    "read_all",
+    "profile:read_all",
+    "profile:write",
+    "activity:read",
+    "activity:read_all",
+    "activity:write",
+]
+
+
+class AccessInfo(TypedDict):
+    """Dictionary containing token exchange response from Strava."""
+
+    access_token: str
+    """A short live token the access Strava API"""
+
+    refresh_token: str
+    """The refresh token for this user, to be used to get the next access token for this
+    user. Please expect that this value can change anytime you retrieve a new access
+    token. Once a new refresh token code has been returned, the older code will no
+    longer work.
+    """
+
+    expires_at: int
+    """The number of seconds since the epoch when the provided access token will expire"""
+
 
 class ApiV3(metaclass=abc.ABCMeta):
     """
     This class is responsible for performing the HTTP requests, rate limiting, and error handling.
     """
 
     server = "www.strava.com"
     api_base = "/api/v3"
 
     def __init__(
-        self, access_token=None, requests_session=None, rate_limiter=None
+        self,
+        access_token: str | None = None,
+        requests_session: requests.Session | None = None,
+        rate_limiter: Callable[[dict[str, str]], None] | None = None,
     ):
         """
         Initialize this protocol client, optionally providing a (shared) :class:`requests.Session`
         object.
 
         :param access_token: The token that provides access to a specific Strava account.
         :type access_token: str
@@ -35,33 +71,33 @@
         :type requests_session::class:`requests.Session`
         """
         self.log = logging.getLogger(
             "{0.__module__}.{0.__name__}".format(self.__class__)
         )
         self.access_token = access_token
         if requests_session:
-            self.rsession = requests_session
+            self.rsession: requests.Session = requests_session
         else:
             self.rsession = requests.Session()
 
         if rate_limiter is None:
             # Make it a dummy function, so we don't have to check if it's defined before
             # calling it later
-            rate_limiter = lambda x=None: None
+            rate_limiter = lambda x: None
 
         self.rate_limiter = rate_limiter
 
     def authorization_url(
         self,
-        client_id,
-        redirect_uri,
-        approval_prompt="auto",
-        scope=None,
-        state=None,
-    ):
+        client_id: int,
+        redirect_uri: str,
+        approval_prompt: Literal["auto", "force"] = "auto",
+        scope: list[Scope] | Scope | None = None,
+        state: str | None = None,
+    ) -> str:
         """
         Get the URL needed to authorize your application to access a Strava user's information.
 
         See https://developers.strava.com/docs/authentication/
 
         :param client_id: The numeric developer client id.
         :type client_id: int
@@ -100,33 +136,31 @@
             "activity:write",
         }
 
         assert not unsupported, "Unsupported scope value(s): {}".format(
             unsupported
         )
 
-        if isinstance(scope, (list, tuple)):
-            scope = ",".join(scope)
-
         params = {
             "client_id": client_id,
             "redirect_uri": redirect_uri,
             "approval_prompt": approval_prompt,
+            "scope": ",".join(scope),
             "response_type": "code",
         }
-        if scope is not None:
-            params["scope"] = scope
         if state is not None:
             params["state"] = state
 
         return urlunsplit(
             ("https", self.server, "/oauth/authorize", urlencode(params), "")
         )
 
-    def exchange_code_for_token(self, client_id, client_secret, code):
+    def exchange_code_for_token(
+        self, client_id: int, client_secret: str, code: str
+    ) -> AccessInfo:
         """
         Exchange the temporary authorization code (returned with redirect from strava authorization URL)
         for a short-lived access token and a refresh token (used to obtain the next access token later on).
 
         :param client_id: The numeric developer client id.
         :type client_id: int
 
@@ -146,23 +180,25 @@
                 "client_id": client_id,
                 "client_secret": client_secret,
                 "code": code,
                 "grant_type": "authorization_code",
             },
             method="POST",
         )
-        access_info = dict()
-        access_info["access_token"] = response["access_token"]
-        access_info["refresh_token"] = response.get("refresh_token", None)
-        access_info["expires_at"] = response.get("expires_at", None)
+        access_info: AccessInfo = {
+            "access_token": response["access_token"],
+            "refresh_token": response["refresh_token"],
+            "expires_at": response["expires_at"],
+        }
         self.access_token = response["access_token"]
-
         return access_info
 
-    def refresh_access_token(self, client_id, client_secret, refresh_token):
+    def refresh_access_token(
+        self, client_id: int, client_secret: str, refresh_token: str
+    ) -> AccessInfo:
         """
         Exchanges the previous refresh token for a short-lived access token and a new
         refresh token (used to obtain the next access token later on).
 
         :param client_id: The numeric developer client id.
         :type client_id: int
 
@@ -182,33 +218,39 @@
                 "client_id": client_id,
                 "client_secret": client_secret,
                 "refresh_token": refresh_token,
                 "grant_type": "refresh_token",
             },
             method="POST",
         )
-        access_info = dict()
-        access_info["access_token"] = response["access_token"]
-        access_info["refresh_token"] = response["refresh_token"]
-        access_info["expires_at"] = response["expires_at"]
+        access_info: AccessInfo = {
+            "access_token": response["access_token"],
+            "refresh_token": response["refresh_token"],
+            "expires_at": response["expires_at"],
+        }
         self.access_token = response["access_token"]
 
         return access_info
 
-    def resolve_url(self, url):
+    def resolve_url(self, url: str) -> str:
         if not url.startswith("http"):
             url = urljoin(
                 "https://{0}".format(self.server),
                 self.api_base + "/" + url.strip("/"),
             )
         return url
 
     def _request(
-        self, url, params=None, files=None, method="GET", check_for_errors=True
-    ):
+        self,
+        url: str,
+        params: dict[str, Any] | None = None,
+        files: dict[str, SupportsRead[str | bytes]] | None = None,
+        method: Literal["GET", "POST", "PUT", "DELETE"] = "GET",
+        check_for_errors: bool = True,
+    ) -> Any:
         """
         Perform the underlying request, returning the parsed JSON results.
 
         :param url: The request URL.
         :type url: str
 
         :param params: Request parameters
@@ -249,15 +291,15 @@
         except KeyError:
             raise ValueError(
                 "Invalid/unsupported request method specified: {0}".format(
                     method
                 )
             )
 
-        raw = requester(url, params=params)
+        raw = requester(url, params=params)  # type: ignore[operator]
         # Rate limits are taken from HTTP response headers
         # https://developers.strava.com/docs/rate-limits/
         self.rate_limiter(raw.headers)
 
         if check_for_errors:
             self._handle_protocol_error(raw)
 
@@ -265,15 +307,17 @@
         if raw.status_code in [204]:
             resp = {}
         else:
             resp = raw.json()
 
         return resp
 
-    def _handle_protocol_error(self, response):
+    def _handle_protocol_error(
+        self, response: requests.Response
+    ) -> requests.Response:
         """
         Parses the raw response from the server, raising a :class:`stravalib.exc.Fault` if the
         server returned an error.
 
         :param response: The response object.
         :raises Fault: If the response contains an error.
         """
@@ -286,79 +330,82 @@
             if "message" in json_response or "errors" in json_response:
                 error_str = "{0}: {1}".format(
                     json_response.get("message", "Undefined error"),
                     json_response.get("errors"),
                 )
 
         # Special subclasses for some errors
-        msg = None
-        exc_class = None
         if response.status_code == 404:
             msg = "%s: %s" % (response.reason, error_str)
-            exc_class = exc.ObjectNotFound
+            raise exc.ObjectNotFound(msg, response=response)
         elif response.status_code == 401:
             msg = "%s: %s" % (response.reason, error_str)
-            exc_class = exc.AccessUnauthorized
+            raise exc.AccessUnauthorized(msg, response=response)
         elif 400 <= response.status_code < 500:
             msg = "%s Client Error: %s [%s]" % (
                 response.status_code,
                 response.reason,
                 error_str,
             )
-            exc_class = exc.Fault
+            raise exc.Fault(msg, response=response)
         elif 500 <= response.status_code < 600:
             msg = "%s Server Error: %s [%s]" % (
                 response.status_code,
                 response.reason,
                 error_str,
             )
-            exc_class = exc.Fault
+            raise exc.Fault(msg, response=response)
         elif error_str:
             msg = error_str
-            exc_class = exc.Fault
-
-        if exc_class is not None:
-            raise exc_class(msg, response=response)
+            raise exc.Fault(msg, response=response)
 
         return response
 
-    def _extract_referenced_vars(self, s):
+    def _extract_referenced_vars(self, s: str) -> list[str]:
         """
         Utility method to find the referenced format variables in a string.
         (Assumes string.format() format vars.)
         :param s: The string that contains format variables. (e.g. "{foo}-text")
         :return: The list of referenced variable names. (e.g. ['foo'])
         :rtype: list
         """
-        d = {}
+        d: dict[str, int] = {}
         while True:
             try:
                 s.format(**d)
             except KeyError as exc:
                 # exc.args[0] contains the name of the key that was not found;
                 # 0 is used because it appears to work with all types of placeholders.
                 d[exc.args[0]] = 0
             else:
                 break
-        return d.keys()
+        return list(d.keys())
 
-    def get(self, url, check_for_errors=True, **kwargs):
+    def get(
+        self, url: str, check_for_errors: bool = True, **kwargs: Any
+    ) -> Any:
         """
         Performs a generic GET request for specified params, returning the response.
         """
         referenced = self._extract_referenced_vars(url)
         url = url.format(**kwargs)
         params = dict(
             [(k, v) for k, v in kwargs.items() if not k in referenced]
         )
         return self._request(
             url, params=params, check_for_errors=check_for_errors
         )
 
-    def post(self, url, files=None, check_for_errors=True, **kwargs):
+    def post(
+        self,
+        url: str,
+        files: dict[str, SupportsRead[str | bytes]] | None = None,
+        check_for_errors: bool = True,
+        **kwargs: Any,
+    ) -> Any:
         """
         Performs a generic POST request for specified params, returning the response.
         """
         referenced = self._extract_referenced_vars(url)
         url = url.format(**kwargs)
         params = dict(
             [(k, v) for k, v in kwargs.items() if not k in referenced]
@@ -367,28 +414,32 @@
             url,
             params=params,
             files=files,
             method="POST",
             check_for_errors=check_for_errors,
         )
 
-    def put(self, url, check_for_errors=True, **kwargs):
+    def put(
+        self, url: str, check_for_errors: bool = True, **kwargs: Any
+    ) -> Any:
         """
         Performs a generic PUT request for specified params, returning the response.
         """
         referenced = self._extract_referenced_vars(url)
         url = url.format(**kwargs)
         params = dict(
             [(k, v) for k, v in kwargs.items() if not k in referenced]
         )
         return self._request(
             url, params=params, method="PUT", check_for_errors=check_for_errors
         )
 
-    def delete(self, url, check_for_errors=True, **kwargs):
+    def delete(
+        self, url: str, check_for_errors: bool = True, **kwargs: Any
+    ) -> Any:
         """
         Performs a generic DELETE request for specified params, returning the response.
         """
         referenced = self._extract_referenced_vars(url)
         url = url.format(**kwargs)
         params = dict(
             [(k, v) for k, v in kwargs.items() if not k in referenced]
```

### Comparing `stravalib-1.3.1/stravalib/strava_model.py` & `stravalib-1.3.2/stravalib/strava_model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/__init__.py` & `stravalib-1.3.2/stravalib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/auth_responder.py` & `stravalib-1.3.2/stravalib/tests/auth_responder.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/functional/__init__.py` & `stravalib-1.3.2/stravalib/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/functional/test_client.py` & `stravalib-1.3.2/stravalib/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/functional/test_client_rate_limiter.py` & `stravalib-1.3.2/stravalib/tests/functional/test_client_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/functional/test_client_write.py` & `stravalib-1.3.2/stravalib/tests/functional/test_client_write.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/functional/test_result_iterator.py` & `stravalib-1.3.2/stravalib/tests/functional/test_result_iterator.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/integration/strava_api_stub.py` & `stravalib-1.3.2/stravalib/tests/integration/strava_api_stub.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/integration/test_client.py` & `stravalib-1.3.2/stravalib/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/activity-manual.3.json` & `stravalib-1.3.2/stravalib/tests/resources/activity-manual.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/activity.3.json` & `stravalib-1.3.2/stravalib/tests/resources/activity.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/athlete.2.json` & `stravalib-1.3.2/stravalib/tests/resources/athlete.2.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/athlete.3.json` & `stravalib-1.3.2/stravalib/tests/resources/athlete.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/example_route_response.json` & `stravalib-1.3.2/stravalib/tests/resources/example_route_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/example_zone_response.json` & `stravalib-1.3.2/stravalib/tests/resources/example_zone_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/sample.tcx` & `stravalib-1.3.2/stravalib/tests/resources/sample.tcx`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/resources/strava_swagger.json` & `stravalib-1.3.2/stravalib/tests/resources/strava_swagger.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/unit/test_client_utils.py` & `stravalib-1.3.2/stravalib/tests/unit/test_client_utils.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/unit/test_field_conversions.py` & `stravalib-1.3.2/stravalib/tests/unit/test_field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/unit/test_limiter.py` & `stravalib-1.3.2/stravalib/tests/unit/test_limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/unit/test_model.py` & `stravalib-1.3.2/stravalib/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/tests/unit/test_unithelper.py` & `stravalib-1.3.2/stravalib/tests/unit/test_unithelper.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/unithelper.py` & `stravalib-1.3.2/stravalib/unithelper.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.1/stravalib/util/limiter.py` & `stravalib-1.3.2/stravalib/util/limiter.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,40 +14,47 @@
   Strava API usage is limited on a per-application basis using a short term,
   15 minute, limit and a long term, daily, limit. The default rate limit allows
   600 requests every 15 minutes, with up to 30,000 requests per day.
 
   This limit allows applications to make 40 requests per minute for about
   half the day.
 """
+from __future__ import annotations
+
 import collections
 import logging
 import time
 from datetime import datetime, timedelta
+from logging import Logger
+from typing import Callable, Deque, Literal, NamedTuple, NoReturn, TypedDict
 
 import arrow
 
 from stravalib import exc
 
 
-def total_seconds(td):
-    """Alternative to datetime.timedelta.total_seconds
-    total_seconds() only available since Python 2.7
-    https://docs.python.org/2/library/datetime.html#datetime.timedelta.total_seconds
-    """
-    return (
-        td.microseconds + (td.seconds + td.days * 24 * 3600) * 10**6
-    ) / 10**6
+class RequestRate(NamedTuple):
+    """Tuple about the request usage and usage limit."""
+
+    short_usage: int
+    """15-minute usage"""
 
+    long_usage: int
+    """Daily usage"""
 
-RequestRate = collections.namedtuple(
-    "RequestRate", ["short_usage", "long_usage", "short_limit", "long_limit"]
-)
+    short_limit: int
+    """15-minutes limit"""
 
+    long_limit: int
+    """Daily limit"""
 
-def get_rates_from_response_headers(headers):
+
+def get_rates_from_response_headers(
+    headers: dict[str, str]
+) -> RequestRate | None:
     """
     Returns a namedtuple with values for short - and long usage and limit rates found in provided HTTP response headers
     :param headers: HTTP response headers
     :type headers: dict
     :return: namedtuple with request rates or None if no rate-limit headers present in response.
     :rtype: Optional[RequestRate]
     """
@@ -61,15 +68,17 @@
             short_limit=limit_rates[0],
             long_limit=limit_rates[1],
         )
     except KeyError:
         return None
 
 
-def get_seconds_until_next_quarter(now=None):
+def get_seconds_until_next_quarter(
+    now: arrow.arrow.Arrow | None = None,
+) -> int:
     """
     Returns the number of seconds until the next quarter of an hour. This is the short-term rate limit used by Strava.
     :param now: A (utc) timestamp
     :type now: arrow.arrow.Arrow
     :return: the number of seconds until the next quarter, as int
     """
     if now is None:
@@ -81,54 +90,91 @@
             - now.replace(
                 minute=(now.minute // 15) * 15, second=0, microsecond=0
             )
         ).seconds
     )
 
 
-def get_seconds_until_next_day(now=None):
+def get_seconds_until_next_day(now: arrow.arrow.Arrow | None = None) -> int:
     """
     Returns the number of seconds until the next day (utc midnight). This is the long-term rate limit used by Strava.
     :param now: A (utc) timestamp
     :type now: arrow.arrow.Arrow
     :return: the number of seconds until next day, as int
     """
     if now is None:
         now = arrow.utcnow()
     return (now.ceil("day") - now).seconds
 
 
-class XRateLimitRule(object):
-    def __init__(self, limits, force_limits=False):
+class LimitStructure(TypedDict):
+    """
+    Dictionary that holds rate limits for a specific time window size.
+    """
+
+    usage: int
+    """Usage in the current period"""
+
+    limit: int
+    """Limit for the period"""
+
+    time: float
+    """Duration of the period"""
+
+    lastExceeded: datetime | None
+    """Last time the limit was exceeded"""
+
+
+class LimitsStructure(TypedDict):
+    """
+    Dictionary that holds rate limiting information for both of strava 15-minutes and
+    daily rate limits.
+    """
+
+    short: LimitStructure
+    """15-minutes rate limiting data"""
+
+    long: LimitStructure
+    """Daily rate limiting data"""
+
+
+class XRateLimitRule:
+    def __init__(
+        self, limits: LimitsStructure, force_limits: bool = False
+    ) -> None:
         """
 
-        :param limits: THe limits structure.
-        :param force_limits: If False (default), this rule will set/update its limits based on what the Strava API
-        tells it. If True, the provided limits will be enforced, i.e. ignoring the limits given by the API.
+        :param limits: The limits structure.
+        :param force_limits:
+            If False (default), this rule will set/update its limits based on
+            what the Strava API tells it.
+            If True, the provided limits will be enforced,
+            i.e. ignoring the limits given by the API.
         """
         self.log = logging.getLogger(
             "{0.__module__}.{0.__name__}".format(self.__class__)
         )
         self.rate_limits = limits
         # should limit args be validated?
-        self.limit_time_invalid = 0
+        self.limit_time_invalid: float = 0.0
         self.force_limits = force_limits
 
     @property
-    def limit_timeout(self):
+    def limit_timeout(self) -> float:
         return self.limit_time_invalid
 
-    def __call__(self, response_headers):
+    def __call__(self, response_headers: dict[str, str]) -> None:
         self._update_usage(response_headers)
 
-        for limit in self.rate_limits.values():
-            self._check_limit_time_invalid(limit)
-            self._check_limit_rates(limit)
+        self._check_limit_time_invalid(self.rate_limits["short"])
+        self._check_limit_rates(self.rate_limits["short"])
+        self._check_limit_time_invalid(self.rate_limits["long"])
+        self._check_limit_rates(self.rate_limits["long"])
 
-    def _update_usage(self, response_headers):
+    def _update_usage(self, response_headers: dict[str, str]) -> None:
         rates = get_rates_from_response_headers(response_headers)
 
         if rates:
             self.log.debug(
                 "Updating rate-limit limits and usage from headers: {}".format(
                     rates
                 )
@@ -136,67 +182,71 @@
             self.rate_limits["short"]["usage"] = rates.short_usage
             self.rate_limits["long"]["usage"] = rates.long_usage
 
             if not self.force_limits:
                 self.rate_limits["short"]["limit"] = rates.short_limit
                 self.rate_limits["long"]["limit"] = rates.long_limit
 
-    def _check_limit_rates(self, limit):
+    def _check_limit_rates(self, limit: LimitStructure) -> None:
         if limit["usage"] >= limit["limit"]:
             self.log.debug("Rate limit of {0} reached.".format(limit["limit"]))
             limit["lastExceeded"] = datetime.now()
             self._raise_rate_limit_exception(limit["limit"], limit["time"])
 
-    def _check_limit_time_invalid(self, limit):
+    def _check_limit_time_invalid(self, limit: LimitStructure) -> None:
         self.limit_time_invalid = 0
         if limit["lastExceeded"] is not None:
             delta = (datetime.now() - limit["lastExceeded"]).total_seconds()
             if delta < limit["time"]:
                 self.limit_time_invalid = limit["time"] - delta
                 self.log.debug(
                     "Rate limit invalid duration {0} seconds.".format(
                         self.limit_time_invalid
                     )
                 )
                 self._raise_rate_limit_timeout(
                     self.limit_timeout, limit["limit"]
                 )
 
-    def _raise_rate_limit_exception(self, timeout, limit_rate):
+    def _raise_rate_limit_exception(
+        self, timeout: float, limit_rate: float
+    ) -> NoReturn:
         raise exc.RateLimitExceeded(
             "Rate limit of {0} exceeded. "
             "Try again in {1} seconds.".format(limit_rate, timeout),
             limit=limit_rate,
             timeout=timeout,
         )
 
-    def _raise_rate_limit_timeout(self, timeout, limit_rate):
+    def _raise_rate_limit_timeout(
+        self, timeout: float, limit_rate: float
+    ) -> NoReturn:
         raise exc.RateLimitTimeout(
-            "Rate limit of {0} exceeded. "
-            "Try again in {1} seconds.".format(limit_rate, timeout),
+            "Rate limit of {} exceeded. "
+            "Try again in {} seconds.".format(limit_rate, timeout),
             limit=limit_rate,
             timeout=timeout,
         )
 
 
-class SleepingRateLimitRule(object):
+class SleepingRateLimitRule:
     """
     A rate limit rule that can be prioritized and can dynamically adapt its limits based on API responses.
     Given its priority, it will enforce a variable "cool-down" period after each response. When rate limits
     are reached within their period, this limiter will wait until the end of that period. It will NOT raise
     any kind of exception in this case.
     """
 
     def __init__(
         self,
-        priority="high",
-        short_limit=10000,
-        long_limit=1000000,
-        force_limits=False,
-    ):
+        priority: Literal["low", "medium", "high"] = "high",
+        short_limit: int = 10000,
+        long_limit: int = 1000000,
+        force_limits: bool = False,
+    ) -> None:
         """
         Constructs a new SleepingRateLimitRule.
         :param priority: The priority for this rule. When 'low', the cool-down period after each request will be such
         that the long-term limits will not be exceeded. When 'medium', the cool-down period will be such that the
         short-term limits will not be exceeded. When 'high', there will be no cool-down period.
         :type priority: str
         :param short_limit: (Optional) explicit short-term limit
@@ -219,34 +269,34 @@
         self.priority = priority
         self.short_limit = short_limit
         self.long_limit = long_limit
         self.force_limits = force_limits
 
     def _get_wait_time(
         self,
-        short_usage,
-        long_usage,
-        seconds_until_short_limit,
-        seconds_until_long_limit,
-    ):
+        short_usage: int,
+        long_usage: int,
+        seconds_until_short_limit: int,
+        seconds_until_long_limit: int,
+    ) -> float:
         if long_usage >= self.long_limit:
             self.log.warning("Long term API rate limit exceeded")
             return seconds_until_long_limit
         elif short_usage >= self.short_limit:
             self.log.warning("Short term API rate limit exceeded")
             return seconds_until_short_limit
 
         if self.priority == "high":
             return 0
         elif self.priority == "medium":
             return seconds_until_short_limit / (self.short_limit - short_usage)
         elif self.priority == "low":
             return seconds_until_long_limit / (self.long_limit - long_usage)
 
-    def __call__(self, response_headers):
+    def __call__(self, response_headers: dict[str, str]) -> None:
         rates = get_rates_from_response_headers(response_headers)
 
         if rates:
             time.sleep(
                 self._get_wait_time(
                     rates.short_usage,
                     rates.long_usage,
@@ -255,30 +305,32 @@
                 )
             )
             if not self.force_limits:
                 self.short_limit = rates.short_limit
                 self.long_limit = rates.long_limit
 
 
-class RateLimitRule(object):
-    def __init__(self, requests, seconds, raise_exc=False):
+class RateLimitRule:
+    def __init__(
+        self, requests: int, seconds: float, raise_exc: bool = False
+    ) -> None:
         """
         :param requests: Number of requests for limit.
         :param seconds: The number of seconds for that number of requests (may be float)
         :param raise_exc: Whether to raise an exception when limit is reached (as opposed to pausing)
         """
         self.log = logging.getLogger(
             "{0.__module__}.{0.__name__}".format(self.__class__)
         )
         self.timeframe = timedelta(seconds=seconds)
         self.requests = requests
-        self.tab = collections.deque(maxlen=self.requests)
+        self.tab: Deque[datetime] = collections.deque(maxlen=self.requests)
         self.raise_exc = raise_exc
 
-    def __call__(self, args):
+    def __call__(self, args: dict[str, str]) -> None:
         """
         Register another request is being issued.
 
         Depending on configuration of the rule will pause if rate limit has
         been reached, or raise exception, etc.
         """
         # First check if the deque is full; that indicates that we'd better check whether
@@ -294,36 +346,32 @@
                         "Rate limit exceeded (can try again in {0})".format(
                             self.timeframe - delta
                         )
                     )
                 else:
                     # Wait the difference between timeframe and the oldest request.
                     td = self.timeframe - delta
-                    sleeptime = (
-                        hasattr(td, "total_seconds")
-                        and td.total_seconds()
-                        or total_seconds(td)
-                    )
+                    sleeptime = td.total_seconds()
                     self.log.debug(
                         "Rate limit triggered; sleeping for {0}".format(
                             sleeptime
                         )
                     )
                     time.sleep(sleeptime)
         self.tab.append(datetime.now())
 
 
-class RateLimiter(object):
-    def __init__(self):
-        self.log = logging.getLogger(
+class RateLimiter:
+    def __init__(self) -> None:
+        self.log: Logger = logging.getLogger(
             "{0.__module__}.{0.__name__}".format(self.__class__)
         )
-        self.rules = []
+        self.rules: list[Callable[[dict[str, str]], None]] = []
 
-    def __call__(self, args):
+    def __call__(self, args: dict[str, str]) -> None:
         """
         Register another request is being issued.
         """
         for r in self.rules:
             r(args)
 
 
@@ -335,37 +383,35 @@
     the limit at midnight, etc.  Will make this more complex in the future.
 
     Strava API usage is limited on a per-application basis using a short term,
     15 minute, limit and a long term, daily, limit. The default rate limit allows
     600 requests every 15 minutes, with up to 30,000 requests per day.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """
         Strava API usage is limited on a per-application basis using a short term,
         15 minute, limit and a long term, daily, limit. The default rate limit
         allows 600 requests every 15 minutes, with up to 30,000 requests per day.
         This limit allows applications to make 40 requests per minute for about half the day.
         """
 
-        super(DefaultRateLimiter, self).__init__()
+        super().__init__()
 
         self.rules.append(
             XRateLimitRule(
                 {
                     "short": {
-                        "usageFieldIndex": 0,
                         "usage": 0,
                         # 60s * 15 = 15 min
                         "limit": 600,
                         "time": (60 * 15),
                         "lastExceeded": None,
                     },
                     "long": {
-                        "usageFieldIndex": 1,
                         "usage": 0,
                         # 60s * 60m * 24 = 1 day
                         "limit": 30000,
                         "time": (60 * 60 * 24),
                         "lastExceeded": None,
                     },
                 }
```

### Comparing `stravalib-1.3.1/stravalib.egg-info/PKG-INFO` & `stravalib-1.3.2/stravalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stravalib
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
 Author-email: Hans Lellelid <hans@xmpl.org>
 Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong
 License: Apache 2.0 License
 Project-URL: homepage, https://example.com
 Project-URL: documentation, https://stravalib.readthedocs.io
 Project-URL: repository, https://github.com/stravalib/stravalib
```

### Comparing `stravalib-1.3.1/stravalib.egg-info/SOURCES.txt` & `stravalib-1.3.2/stravalib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
 .github/workflows/build-docs.yml
 .github/workflows/build-test.yml
 .github/workflows/check-strava-api.yml
 .github/workflows/push-pypi.yml
+.github/workflows/type-check.yml
 docs/Makefile
 docs/conf.py
 docs/index.md
 docs/reference.rst
 docs/_static/keepme
 docs/_static/stravalib.css
 docs/contributing/build-release-guide.md
@@ -101,22 +102,24 @@
 docs/reference/api/stravalib.field_conversions.timezone.rst
 docs/reference/api/stravalib.unithelper.Quantity.rst
 docs/reference/api/stravalib.unithelper.UnitConverter.rst
 docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
 docs/reference/api/stravalib.unithelper.c2f.rst
 docs/reference/api/stravalib.unithelper.is_quantity_type.rst
 docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
+docs/reference/api/stravalib.util.limiter.LimitStructure.rst
+docs/reference/api/stravalib.util.limiter.LimitsStructure.rst
 docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
 docs/reference/api/stravalib.util.limiter.RateLimiter.rst
+docs/reference/api/stravalib.util.limiter.RequestRate.rst
 docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
 docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
 docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
 docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
 docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
-docs/reference/api/stravalib.util.limiter.total_seconds.rst
 examples/strava-oauth/README.md
 examples/strava-oauth/requirements.txt
 examples/strava-oauth/server.py
 examples/strava-oauth/static/ConnectWithStrava.png
 examples/strava-oauth/templates/login.html
 examples/strava-oauth/templates/login_error.html
 examples/strava-oauth/templates/login_results.html
```

