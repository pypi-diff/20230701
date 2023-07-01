# Comparing `tmp/stravalib-1.3.2.tar.gz` & `tmp/stravalib-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stravalib-1.3.2.tar", last modified: Sat Jul  1 08:08:46 2023, max compression
+gzip compressed data, was "stravalib-1.3.3.tar", last modified: Sat Jul  1 08:53:11 2023, max compression
```

## Comparing `stravalib-1.3.2.tar` & `stravalib-1.3.3.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 08:08:30.000000 stravalib-1.3.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-01 08:08:30.000000 stravalib-1.3.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/build-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/check-strava-api.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/push-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-01 08:08:30.000000 stravalib-1.3.2/.github/workflows/type-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-01 08:08:30.000000 stravalib-1.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-01 08:08:30.000000 stravalib-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 08:08:30.000000 stravalib-1.3.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-01 08:08:30.000000 stravalib-1.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-01 08:08:30.000000 stravalib-1.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-01 08:08:30.000000 stravalib-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 08:08:30.000000 stravalib-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-01 08:08:30.000000 stravalib-1.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-01 08:08:46.844701 stravalib-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-01 08:08:30.000000 stravalib-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-01 08:08:30.000000 stravalib-1.3.2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/_static/keepme
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/_static/stravalib.css
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/build-release-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/development-guide.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/documentation-changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/how-to-contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/contributing/resources-for-new-contributors.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/athletes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/authenticate-with-strava.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/get-started/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/images/stravalib_architecture.png
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.828701 stravalib-1.3.2/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/docs/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.ActivityUploader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.ActivityUploader.update_from_response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.BatchedResultsIterator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.authorization_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.create_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.create_subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.deauthorize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.delete_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.delete_subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.exchange_code_for_token.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.explore_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_comments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_kudos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_laps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_photos.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_activity_zones.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_clubs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_koms.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_starred_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_athlete_stats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_club_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_club_members.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_effort_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_friend_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_gear.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_related_activities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_route.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_route_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_routes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment_effort.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment_efforts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_segment_streams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.get_starred_segments.rst
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.handle_subscription_callback.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.handle_subscription_update.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.join_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.leave_club.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.list_subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.refresh_access_token.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.update_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.update_athlete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.client.Client.upload_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.enum_value.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.enum_values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.optional_input.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.time_interval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.field_conversions.timezone.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.Quantity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.UnitConverter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.c2f.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.unithelper.is_quantity_type.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.LimitStructure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.LimitsStructure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.RateLimiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.RequestRate.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/field-conversions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/strava_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/unithelper.rst
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-01 08:08:30.000000 stravalib-1.3.2/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 08:08:30.000000 stravalib-1.3.2/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.824701 stravalib-1.3.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/examples/strava-oauth/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/examples/strava-oauth/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/static/ConnectWithStrava.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.836701 stravalib-1.3.2/examples/strava-oauth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/templates/login_error.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-01 08:08:30.000000 stravalib-1.3.2/examples/strava-oauth/templates/login_results.html
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 08:08:30.000000 stravalib-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-01 08:08:30.000000 stravalib-1.3.2/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 08:08:30.000000 stravalib-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:08:46.844701 stravalib-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib/_version_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)    69653 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    36042 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/strava_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/auth_responder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_client_rate_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_client_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/functional/test_result_iterator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/strava_api_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)    24592 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/integration/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/stravalib/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/activity-manual.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/activity.3.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/athlete.2.json
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/athlete.3.json
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/example_route_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/example_zone_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   451575 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/sample.tcx
--rw-r--r--   0 runner    (1001) docker     (123)   102646 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/resources/strava_swagger.json
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/test.ini-example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/stravalib/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_field_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/tests/unit/test_unithelper.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/unit_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/unithelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.844701 stravalib-1.3.2/stravalib/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-01 08:08:30.000000 stravalib-1.3.2/stravalib/util/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:08:46.840701 stravalib-1.3.2/stravalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 08:08:46.000000 stravalib-1.3.2/stravalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.370692 stravalib-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-01 08:52:54.000000 stravalib-1.3.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-01 08:52:54.000000 stravalib-1.3.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/workflows/build-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/workflows/check-strava-api.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/workflows/push-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-01 08:52:54.000000 stravalib-1.3.3/.github/workflows/type-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-01 08:52:54.000000 stravalib-1.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-01 08:52:54.000000 stravalib-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 08:52:54.000000 stravalib-1.3.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-01 08:52:54.000000 stravalib-1.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-01 08:52:54.000000 stravalib-1.3.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-01 08:52:54.000000 stravalib-1.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-01 08:52:54.000000 stravalib-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-01 08:52:54.000000 stravalib-1.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-01 08:53:11.370692 stravalib-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-07-01 08:52:54.000000 stravalib-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-01 08:52:54.000000 stravalib-1.3.3/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/_static/keepme
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/_static/stravalib.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/contributing/build-release-guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/contributing/development-guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/contributing/documentation-changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/contributing/how-to-contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/contributing/resources-for-new-contributors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/get-started/activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/get-started/athletes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/get-started/authenticate-with-strava.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/get-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/get-started/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.350691 stravalib-1.3.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    78545 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/images/stravalib_architecture.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.354691 stravalib-1.3.3/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.362691 stravalib-1.3.3/docs/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.ActivityUploader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.ActivityUploader.update_from_response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.BatchedResultsIterator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.authorization_url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.create_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.create_subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.deauthorize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.delete_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.delete_subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.exchange_code_for_token.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.explore_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity_comments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity_kudos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity_laps.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity_photos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_activity_zones.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_athlete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_athlete_clubs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_athlete_koms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_athlete_starred_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_athlete_stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_club_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_club_members.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_effort_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_friend_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_gear.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_related_activities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_route.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_route_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_routes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_segment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_segment_effort.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_segment_efforts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_segment_streams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.get_starred_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.handle_subscription_callback.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.handle_subscription_update.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.join_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.leave_club.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.list_subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.refresh_access_token.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.update_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.update_athlete.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.client.Client.upload_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.field_conversions.enum_value.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.field_conversions.enum_values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.field_conversions.optional_input.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.field_conversions.time_interval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.field_conversions.timezone.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.unithelper.Quantity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.unithelper.UnitConverter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.unithelper.UnitsQuantity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.unithelper.c2f.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.unithelper.is_quantity_type.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.DefaultRateLimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.LimitStructure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.LimitsStructure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.RateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.RateLimiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.RequestRate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.SleepingRateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.XRateLimitRule.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.get_rates_from_response_headers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_day.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.get_seconds_until_next_quarter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/field-conversions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/strava_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/unithelper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-01 08:52:54.000000 stravalib-1.3.3/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-01 08:52:54.000000 stravalib-1.3.3/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.346691 stravalib-1.3.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.362691 stravalib-1.3.3/examples/strava-oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.362691 stravalib-1.3.3/examples/strava-oauth/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/static/ConnectWithStrava.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.362691 stravalib-1.3.3/examples/strava-oauth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/templates/login_error.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-01 08:52:54.000000 stravalib-1.3.3/examples/strava-oauth/templates/login_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-01 08:52:54.000000 stravalib-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-01 08:52:54.000000 stravalib-1.3.3/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-01 08:52:54.000000 stravalib-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 08:53:11.370692 stravalib-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.362691 stravalib-1.3.3/stravalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-01 08:53:11.000000 stravalib-1.3.3/stravalib/_version_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69653 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36042 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/strava_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.366691 stravalib-1.3.3/stravalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/auth_responder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.366691 stravalib-1.3.3/stravalib/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/functional/test_client_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/functional/test_client_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/functional/test_result_iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.366691 stravalib-1.3.3/stravalib/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/integration/strava_api_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24592 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/integration/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.366691 stravalib-1.3.3/stravalib/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/activity-manual.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/activity.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/athlete.2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/athlete.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/example_route_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/example_zone_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   451575 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/sample.tcx
+-rw-r--r--   0 runner    (1001) docker     (123)   102646 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/resources/strava_swagger.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/test.ini-example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.366691 stravalib-1.3.3/stravalib/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/unit/test_client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/unit/test_field_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/unit/test_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/tests/unit/test_unithelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/unit_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/unithelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.366691 stravalib-1.3.3/stravalib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-01 08:52:54.000000 stravalib-1.3.3/stravalib/util/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 08:53:11.362691 stravalib-1.3.3/stravalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-01 08:53:11.000000 stravalib-1.3.3/stravalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-07-01 08:53:11.000000 stravalib-1.3.3/stravalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 08:53:11.000000 stravalib-1.3.3/stravalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 08:53:11.000000 stravalib-1.3.3/stravalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 08:53:11.000000 stravalib-1.3.3/stravalib.egg-info/top_level.txt
```

### Comparing `stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md` & `stravalib-1.3.3/.github/PULL_REQUEST_TEMPLATE/release-pull-request-template.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.github/PULL_REQUEST_TEMPLATE.md` & `stravalib-1.3.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.github/workflows/build-docs.yml` & `stravalib-1.3.3/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.github/workflows/build-test.yml` & `stravalib-1.3.3/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.github/workflows/check-strava-api.yml` & `stravalib-1.3.3/.github/workflows/check-strava-api.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.github/workflows/push-pypi.yml` & `stravalib-1.3.3/.github/workflows/push-pypi.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.github/workflows/type-check.yml` & `stravalib-1.3.3/.github/workflows/type-check.yml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/.pre-commit-config.yaml` & `stravalib-1.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/CODE_OF_CONDUCT.md` & `stravalib-1.3.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/CONTRIBUTING.md` & `stravalib-1.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/LICENSE.txt` & `stravalib-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/Makefile` & `stravalib-1.3.3/Makefile`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/PKG-INFO` & `stravalib-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stravalib
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
 Author-email: Hans Lellelid <hans@xmpl.org>
 Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong
 License: Apache 2.0 License
 Project-URL: homepage, https://example.com
 Project-URL: documentation, https://stravalib.readthedocs.io
 Project-URL: repository, https://github.com/stravalib/stravalib
```

### Comparing `stravalib-1.3.2/README.md` & `stravalib-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/changelog.md` & `stravalib-1.3.3/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Change Log
 
 ## Unreleased
 
+## v1.3.3
+
+### Fixed
+
+- Fix: pins pydantic to v1 in pyproject.toml dependencies (@jsamoocha, #382)
+
 ## v1.3.2
 
 ### Added
 
 - Add: type checking to limiter, protocol and exc file (@enadeau , #374)
 
 ### Fixed
```

### Comparing `stravalib-1.3.2/docs/Makefile` & `stravalib-1.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/conf.py` & `stravalib-1.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/contributing/build-release-guide.md` & `stravalib-1.3.3/docs/contributing/build-release-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/contributing/development-guide.md` & `stravalib-1.3.3/docs/contributing/development-guide.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/contributing/resources-for-new-contributors.md` & `stravalib-1.3.3/docs/contributing/resources-for-new-contributors.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/get-started/activities.rst` & `stravalib-1.3.3/docs/get-started/activities.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/get-started/athletes.rst` & `stravalib-1.3.3/docs/get-started/athletes.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/get-started/authenticate-with-strava.rst` & `stravalib-1.3.3/docs/get-started/authenticate-with-strava.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/get-started/index.md` & `stravalib-1.3.3/docs/get-started/index.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/get-started/overview.rst` & `stravalib-1.3.3/docs/get-started/overview.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/images/stravalib_architecture.png` & `stravalib-1.3.3/docs/images/stravalib_architecture.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/index.md` & `stravalib-1.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/api/stravalib.client.ActivityUploader.rst` & `stravalib-1.3.3/docs/reference/api/stravalib.client.ActivityUploader.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/api/stravalib.client.Client.rst` & `stravalib-1.3.3/docs/reference/api/stravalib.client.Client.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.LimitStructure.rst` & `stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.LimitStructure.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/api/stravalib.util.limiter.LimitsStructure.rst` & `stravalib-1.3.3/docs/reference/api/stravalib.util.limiter.LimitsStructure.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/client.rst` & `stravalib-1.3.3/docs/reference/client.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/model.rst` & `stravalib-1.3.3/docs/reference/model.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference/utilities.rst` & `stravalib-1.3.3/docs/reference/utilities.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/docs/reference.rst` & `stravalib-1.3.3/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/examples/strava-oauth/README.md` & `stravalib-1.3.3/examples/strava-oauth/README.md`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/examples/strava-oauth/server.py` & `stravalib-1.3.3/examples/strava-oauth/server.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/examples/strava-oauth/static/ConnectWithStrava.png` & `stravalib-1.3.3/examples/strava-oauth/static/ConnectWithStrava.png`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/examples/strava-oauth/templates/login.html` & `stravalib-1.3.3/examples/strava-oauth/templates/login.html`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/pyproject.toml` & `stravalib-1.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 dependencies = [
     "pint",
     "pytz",
     "arrow",
     "requests",
-    "pydantic",
+    "pydantic==1.10.9",
 ]
 
 [project.urls]
 homepage = "https://example.com"
 documentation = "https://stravalib.readthedocs.io"
 repository = "https://github.com/stravalib/stravalib"
 changelog = "https://github.com/stravalib/stravalib/blob/master/changelog.md"
```

### Comparing `stravalib-1.3.2/stravalib/client.py` & `stravalib-1.3.3/stravalib/client.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/exc.py` & `stravalib-1.3.3/stravalib/exc.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/field_conversions.py` & `stravalib-1.3.3/stravalib/field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/model.py` & `stravalib-1.3.3/stravalib/model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/protocol.py` & `stravalib-1.3.3/stravalib/protocol.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/strava_model.py` & `stravalib-1.3.3/stravalib/strava_model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/__init__.py` & `stravalib-1.3.3/stravalib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/auth_responder.py` & `stravalib-1.3.3/stravalib/tests/auth_responder.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/functional/__init__.py` & `stravalib-1.3.3/stravalib/tests/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/functional/test_client.py` & `stravalib-1.3.3/stravalib/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/functional/test_client_rate_limiter.py` & `stravalib-1.3.3/stravalib/tests/functional/test_client_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/functional/test_client_write.py` & `stravalib-1.3.3/stravalib/tests/functional/test_client_write.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/functional/test_result_iterator.py` & `stravalib-1.3.3/stravalib/tests/functional/test_result_iterator.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/integration/strava_api_stub.py` & `stravalib-1.3.3/stravalib/tests/integration/strava_api_stub.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/integration/test_client.py` & `stravalib-1.3.3/stravalib/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/activity-manual.3.json` & `stravalib-1.3.3/stravalib/tests/resources/activity-manual.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/activity.3.json` & `stravalib-1.3.3/stravalib/tests/resources/activity.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/athlete.2.json` & `stravalib-1.3.3/stravalib/tests/resources/athlete.2.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/athlete.3.json` & `stravalib-1.3.3/stravalib/tests/resources/athlete.3.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/example_route_response.json` & `stravalib-1.3.3/stravalib/tests/resources/example_route_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/example_zone_response.json` & `stravalib-1.3.3/stravalib/tests/resources/example_zone_response.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/sample.tcx` & `stravalib-1.3.3/stravalib/tests/resources/sample.tcx`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/resources/strava_swagger.json` & `stravalib-1.3.3/stravalib/tests/resources/strava_swagger.json`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/unit/test_client_utils.py` & `stravalib-1.3.3/stravalib/tests/unit/test_client_utils.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/unit/test_field_conversions.py` & `stravalib-1.3.3/stravalib/tests/unit/test_field_conversions.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/unit/test_limiter.py` & `stravalib-1.3.3/stravalib/tests/unit/test_limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/unit/test_model.py` & `stravalib-1.3.3/stravalib/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/tests/unit/test_unithelper.py` & `stravalib-1.3.3/stravalib/tests/unit/test_unithelper.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/unithelper.py` & `stravalib-1.3.3/stravalib/unithelper.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib/util/limiter.py` & `stravalib-1.3.3/stravalib/util/limiter.py`

 * *Files identical despite different names*

### Comparing `stravalib-1.3.2/stravalib.egg-info/PKG-INFO` & `stravalib-1.3.3/stravalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stravalib
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package that makes it easy to access and download data from the Strava V3 REST API.
 Author-email: Hans Lellelid <hans@xmpl.org>
 Maintainer: Leah Wasser, Hans Lellelid, Jonatan Samoocha, Yihong
 License: Apache 2.0 License
 Project-URL: homepage, https://example.com
 Project-URL: documentation, https://stravalib.readthedocs.io
 Project-URL: repository, https://github.com/stravalib/stravalib
```

### Comparing `stravalib-1.3.2/stravalib.egg-info/SOURCES.txt` & `stravalib-1.3.3/stravalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

