
et
EVENT TYPE DESCRIPTION
======================

The list of events captured.

``` 
SELECT DISTINCT (event_name) FROM 'radar-armt-notification.analytics_180955751.events_intraday_20210616'
```


```
 - session_start
 - resumed
 - prepared_kafka_object
 - send_to_cache
 - user_engagement
 - notification_open
 - screen_view
 - notification_refreshed
 - click
 - questionnaire_started
 - questionnaire_finished
 - send_success
 - removed_from_cache
 - recording_started
 - recording_stopped
 - notification_dismiss
 - notification_receive
 - send_error
 - notification_foreground
 - questionnaire_cancelled
 - error
 - app_remove
 - firebase_campaign
 - protocol_change
 - notification_cancelled
 - notification_rescheduled
 - first_open
 - sign_up
 - app_reset
 - qr_code_scanned
 - sign_up_fail
 - notification_test
 - app_version_change
 - config_error
 - timezone_change

```




EVENT DATASET DESCRIPTION
=========================

A join of the tables to get Project ID, Subject ID via an UNNEST and other elements can be provided in BigQuery here:


```
| Row | event_date | event_timestamp  | event_name           | event_param_key       | event_param_int | event_param_string | user_pseudo_id                   | user_prop_key | user_prop_string                     |
|-----|------------|------------------|----------------------|-----------------------|-----------------|--------------------|----------------------------------|---------------|--------------------------------------|
| 1   | 20191208   | 1575779411418000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 2   | 20191208   | 1575779411418000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 3   | 20191208   | 1575779411418000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 4   | 20191208   | 1575779411418000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 5   | 20191208   | 1575779411418000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 6   | 20191208   | 1575779411418000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 7   | 20191208   | 1575781263225000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 8   | 20191208   | 1575781263225000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 9   | 20191208   | 1575781263225000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 10  | 20191208   | 1575781263225000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 11  | 20191208   | 1575781263225000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 12  | 20191208   | 1575781263225000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 13  | 20191208   | 1575783008202000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 14  | 20191208   | 1575783008202000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 15  | 20191208   | 1575783008202000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 16  | 20191208   | 1575783008202000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 17  | 20191208   | 1575783008202000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 18  | 20191208   | 1575783008202000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 19  | 20191208   | 1575785532200000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 20  | 20191208   | 1575785532200000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 21  | 20191208   | 1575785532200000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 22  | 20191208   | 1575785532200000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 23  | 20191208   | 1575785532200000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 24  | 20191208   | 1575785532200000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 25  | 20191208   | 1575786611198000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 26  | 20191208   | 1575786611198000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 27  | 20191208   | 1575786611198000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 28  | 20191208   | 1575786611198000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 29  | 20191208   | 1575786611198000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 30  | 20191208   | 1575786611198000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 31  | 20191208   | 1575790569254000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 32  | 20191208   | 1575790569254000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 33  | 20191208   | 1575790569254000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 34  | 20191208   | 1575790569254000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 35  | 20191208   | 1575790569254000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 36  | 20191208   | 1575790569254000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 37  | 20191208   | 1575803946376000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 38  | 20191208   | 1575803946376000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 39  | 20191208   | 1575803946376000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 40  | 20191208   | 1575803946376000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 41  | 20191208   | 1575803946376000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 42  | 20191208   | 1575803946376000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 43  | 20191208   | 1575810011231000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 44  | 20191208   | 1575810011231000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 45  | 20191208   | 1575810011231000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 46  | 20191208   | 1575810011231000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 47  | 20191208   | 1575810011231000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 48  | 20191208   | 1575810011231000 | notification_receive | firebase_conversion   | 1               | null               | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | subjectId     | ae5xxxxx-xxxx-xxxx-xxxx-xxxxxxxxx04b |
| 49  | 20191208   | 1575814625219000 | notification_receive | message_type          | null            | display            | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
| 50  | 20191208   | 1575814625219000 | notification_receive | firebase_event_origin | null            | fcm                | 3c8xxxxxxxxxxxxxxxxxxxxxxxxxa1e6 | projectId     | STAGING_PROJECT                      |
```


Yatharth's suggests using the Python API (which should simplify getting stuff into a Pandas or similar) [see](https://github.com/afolarin/Firebase-events-analysis/blob/master/.ipynb_checkpoints/bigquery-explore-checkpoint.ipynb)
```
def get_query(table_name: str, start_date: str, end_date: str) -> str:
    return f"""
        SELECT 
         event_date,
         event_timestamp, 
         event_name, 
         event_parameters.key AS event_param_key, 
         event_parameters.value.int_value AS event_param_int, 
         event_parameters.value.string_value AS event_param_string,
         user_pseudo_id, 
         user_prop.key AS user_prop_key, 
         user_prop.value.string_value AS user_prop_string
        FROM
         `{table_name}` as T,
          UNNEST(user_properties) AS user_prop,
          UNNEST(event_params) AS event_parameters
        WHERE 
          _TABLE_SUFFIX BETWEEN "{start_date}" AND "{end_date}"
          AND ((event_name = "user_engagement" AND event_parameters.key = "engagement_time_msec") OR (event_name = "notification_receive") OR event_name = "notification_open")
          AND (user_prop.key = "subjectId" OR user_prop.key = "projectId")
    """
```


# Reorganise by Project pre_process()

|index                     |event_date|event_timestamp |event_name          |user_pseudo_id                  |subjectId                           |engagement_time_msec|message_type|projectId      |
|--------------------------|----------|----------------|--------------------|--------------------------------|------------------------------------|--------------------|------------|---------------|
|2019-12-03 08:00:02.811000|20191203  |1575360002811000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 08:00:02.811000|20191203  |1575360002811000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 08:00:02.811000|20191203  |1575360002811000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 08:00:02.887001|20191203  |1575360002887001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 08:00:02.887001|20191203  |1575360002887001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 08:00:02.887001|20191203  |1575360002887001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 09:00:08.079000|20191203  |1575363608079000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 09:00:08.079000|20191203  |1575363608079000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 09:00:08.079000|20191203  |1575363608079000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 09:00:08.154001|20191203  |1575363608154001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 09:00:08.154001|20191203  |1575363608154001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 09:00:08.154001|20191203  |1575363608154001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 09:00:08.203002|20191203  |1575363608203002|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 09:00:08.203002|20191203  |1575363608203002|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 09:00:08.203002|20191203  |1575363608203002|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 10:00:03.669000|20191203  |1575367203669000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 10:00:03.669000|20191203  |1575367203669000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 10:00:03.669000|20191203  |1575367203669000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 11:00:06.961000|20191203  |1575370806961000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 11:00:06.961000|20191203  |1575370806961000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 11:00:06.961000|20191203  |1575370806961000|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 11:00:07.034001|20191203  |1575370807034001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |display     |STAGING_PROJECT|
|2019-12-03 11:00:07.034001|20191203  |1575370807034001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|                    |fcm         |STAGING_PROJECT|
|2019-12-03 11:00:07.034001|20191203  |1575370807034001|notification_receive|9a04xxxxxxxxxxxxxxxxxxxxxxxe15b|eee17b85-xxxx-xxxx-xxxx-e9d5dd557dd6|1                   |            |STAGING_PROJECT|
|2019-12-03 10:00:04.135000|20191203  |1575367204135000|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|                    |display     |STAGING_PROJECT|
|2019-12-03 10:00:04.135000|20191203  |1575367204135000|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|                    |fcm         |STAGING_PROJECT|
|2019-12-03 10:00:04.135000|20191203  |1575367204135000|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|1                   |            |STAGING_PROJECT|
|2019-12-03 11:00:09.121000|20191203  |1575370809121000|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|                    |display     |STAGING_PROJECT|
|2019-12-03 11:00:09.121000|20191203  |1575370809121000|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|                    |fcm         |STAGING_PROJECT|
|2019-12-03 11:00:09.121000|20191203  |1575370809121000|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|1                   |            |STAGING_PROJECT|
|2019-12-03 11:00:09.180001|20191203  |1575370809180001|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|                    |display     |STAGING_PROJECT|
|2019-12-03 11:00:09.180001|20191203  |1575370809180001|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|                    |fcm         |STAGING_PROJECT|
|2019-12-03 11:00:09.180001|20191203  |1575370809180001|notification_receive|d08c92ba50feeda04dbac079ca578850|acbd725c-545d-4a8b-bd8d-9b03db18a423|1                   |            |STAGING_PROJECT|
|2020-04-12 11:31:22.037001|20200412  |1586691082037001|user_engagement     |42FBD864C0934CB1B8F68CC990309069|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|1332                |            |STAGING_PROJECT|
|2020-04-12 11:31:22.794004|20200412  |1586691082794004|user_engagement     |42FBD864C0934CB1B8F68CC990309069|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|756                 |            |STAGING_PROJECT|
|2020-04-12 10:25:27.366002|20200412  |1586687127366002|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|11980               |            |STAGING_PROJECT|
|2020-04-12 10:25:39.563017|20200412  |1586687139563017|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|12199               |            |STAGING_PROJECT|
|2020-04-12 10:25:44.611024|20200412  |1586687144611024|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|4942                |            |STAGING_PROJECT|
|2020-04-12 10:26:03.844033|20200412  |1586687163844033|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|18999               |            |STAGING_PROJECT|
|2020-04-12 10:26:11.845053|20200412  |1586687171845053|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|8356                |            |STAGING_PROJECT|
|2020-04-12 10:26:14.185059|20200412  |1586687174185059|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|2339                |            |STAGING_PROJECT|
|2020-04-12 10:26:27.223064|20200412  |1586687187223064|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|13035               |            |STAGING_PROJECT|
|2020-04-12 10:27:24.103067|20200412  |1586687244103067|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|1820                |            |STAGING_PROJECT|
|2020-04-12 10:27:28.237070|20200412  |1586687248237070|user_engagement     |bc0787e6a3a025f641e0fcb2f98bb2f0|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|812                 |            |STAGING_PROJECT|
|2020-04-12 10:31:25.138002|20200412  |1586687485138002|user_engagement     |836faf8525c94da7cd0ae69bf9fbc5b2|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|4761                |            |STAGING_PROJECT|
|2020-04-12 10:31:37.646007|20200412  |1586687497646007|user_engagement     |836faf8525c94da7cd0ae69bf9fbc5b2|2b9f23d2-78cb-4ca4-9e98-6ab1219fb1b5|12491               |            |STAGING_PROJECT|





