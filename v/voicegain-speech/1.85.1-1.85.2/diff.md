# Comparing `tmp/voicegain-speech-1.85.1.tar.gz` & `tmp/voicegain-speech-1.85.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicegain-speech-1.85.1.tar", last modified: Thu Jun 29 21:55:29 2023, max compression
+gzip compressed data, was "voicegain-speech-1.85.2.tar", last modified: Fri Jun 30 03:38:40 2023, max compression
```

## Comparing `voicegain-speech-1.85.1.tar` & `voicegain-speech-1.85.2.tar`

### file list

```diff
@@ -1,478 +1,478 @@
-drwxr-xr-x   0     1001     1002        0 2023-06-29 21:55:29.096396 voicegain-speech-1.85.1/
--rw-r--r--   0     1001     1002    11357 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/LICENSE
--rw-r--r--   0     1001     1002     2923 2023-06-29 21:55:29.096396 voicegain-speech-1.85.1/PKG-INFO
--rw-r--r--   0     1001     1002     2491 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/README.md
--rw-r--r--   0     1001     1002       79 2023-06-29 21:55:29.096396 voicegain-speech-1.85.1/setup.cfg
--rw-r--r--   0     1001     1002      709 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/setup.py
-drwxr-xr-x   0     1001     1002        0 2023-06-29 21:55:29.008389 voicegain-speech-1.85.1/voicegain_speech/
--rw-r--r--   0     1001     1002    63205 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/__init__.py
-drwxr-xr-x   0     1001     1002        0 2023-06-29 21:55:29.012389 voicegain-speech-1.85.1/voicegain_speech/api/
--rw-r--r--   0     1001     1002      821 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/__init__.py
--rw-r--r--   0     1001     1002    33296 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/aivr_api.py
--rw-r--r--   0     1001     1002    52231 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/aivr_callback_api.py
--rw-r--r--   0     1001     1002    39239 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/asr_callback_api.py
--rw-r--r--   0     1001     1002    34611 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/audiocodes_api.py
--rw-r--r--   0     1001     1002   107541 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/data_api.py
--rw-r--r--   0     1001     1002   143654 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/greg_api.py
--rw-r--r--   0     1001     1002    63228 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/lm_api.py
--rw-r--r--   0     1001     1002    48177 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/recognize_api.py
--rw-r--r--   0     1001     1002   118990 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/sa_api.py
--rw-r--r--   0     1001     1002    37190 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/security_api.py
--rw-r--r--   0     1001     1002    57369 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/training_api.py
--rw-r--r--   0     1001     1002   103246 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/transcribe_api.py
--rw-r--r--   0     1001     1002    55744 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api/websocket_api.py
--rw-r--r--   0     1001     1002    51954 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/api_client.py
--rw-r--r--   0     1001     1002    38411 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/configuration.py
--rw-r--r--   0     1001     1002    30458 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/exceptions.py
-drwxr-xr-x   0     1001     1002        0 2023-06-29 21:55:29.096396 voicegain-speech-1.85.1/voicegain_speech/models/
--rw-r--r--   0     1001     1002    62021 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/__init__.py
--rw-r--r--   0     1001     1002    40147 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_control_messages.py
--rw-r--r--   0     1001     1002    31410 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_end.py
--rw-r--r--   0     1001     1002    31418 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_error.py
--rw-r--r--   0     1001     1002    31536 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_hypothesis.py
--rw-r--r--   0     1001     1002    30265 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_hypothesis_alternatives.py
--rw-r--r--   0     1001     1002    31506 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_recognition.py
--rw-r--r--   0     1001     1002    31669 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_recognition_alternatives.py
--rw-r--r--   0     1001     1002    32543 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_response_messages.py
--rw-r--r--   0     1001     1002    39630 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_start.py
--rw-r--r--   0     1001     1002    31682 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_start_stt_speech_contexts.py
--rw-r--r--   0     1001     1002    30535 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_started.py
--rw-r--r--   0     1001     1002    30604 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ac_stop.py
--rw-r--r--   0     1001     1002    31282 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/account_and_context_id.py
--rw-r--r--   0     1001     1002    34185 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/advanced_regex.py
--rw-r--r--   0     1001     1002    30212 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aircall.py
--rw-r--r--   0     1001     1002    30252 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aircall_all_of.py
--rw-r--r--   0     1001     1002    36151 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_callback_response.py
--rw-r--r--   0     1001     1002    31567 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_callback_response_final.py
--rw-r--r--   0     1001     1002    30229 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_conference_transfer.py
--rw-r--r--   0     1001     1002    30887 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_disconnect.py
--rw-r--r--   0     1001     1002    33825 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_event.py
--rw-r--r--   0     1001     1002    29630 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_event_type.py
--rw-r--r--   0     1001     1002    33088 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_existing_session.py
--rw-r--r--   0     1001     1002    32700 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic.py
--rw-r--r--   0     1001     1002    29493 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic_media.py
--rw-r--r--   0     1001     1002    31442 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic_transfer.py
--rw-r--r--   0     1001     1002    29579 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic_type.py
--rw-r--r--   0     1001     1002    41441 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_new_session.py
--rw-r--r--   0     1001     1002    30984 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_phone_transfer.py
--rw-r--r--   0     1001     1002    33974 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt.py
--rw-r--r--   0     1001     1002    30671 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_completion.py
--rw-r--r--   0     1001     1002    35387 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_playing.py
--rw-r--r--   0     1001     1002    30195 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_properties_audio.py
--rw-r--r--   0     1001     1002    30205 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_properties_html.py
--rw-r--r--   0     1001     1002    36852 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_question.py
--rw-r--r--   0     1001     1002    29590 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_recognition_result.py
--rw-r--r--   0     1001     1002    35657 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_recording.py
--rw-r--r--   0     1001     1002    41835 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_response_properties_audio.py
--rw-r--r--   0     1001     1002    31782 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_response_properties_html.py
--rw-r--r--   0     1001     1002    34452 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_session_user.py
--rw-r--r--   0     1001     1002    30558 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_session_user_base.py
--rw-r--r--   0     1001     1002    33324 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_session_user_fs.py
--rw-r--r--   0     1001     1002    32024 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivr_transfer.py
--rw-r--r--   0     1001     1002    32352 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/aivrs_question_specifics.py
--rw-r--r--   0     1001     1002    31632 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/answer_map_entry.py
--rw-r--r--   0     1001     1002    29584 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_event.py
--rw-r--r--   0     1001     1002    29675 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status.py
--rw-r--r--   0     1001     1002    29595 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status_additional.py
--rw-r--r--   0     1001     1002    29650 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status_after_input_started.py
--rw-r--r--   0     1001     1002    29677 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status_for_callback.py
--rw-r--r--   0     1001     1002    29586 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_recognition_result.py
--rw-r--r--   0     1001     1002    42889 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_common.py
--rw-r--r--   0     1001     1002    56905 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition.py
--rw-r--r--   0     1001     1002    52269 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition_defaults.py
--rw-r--r--   0     1001     1002    43582 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
--rw-r--r--   0     1001     1002    38338 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition_timeouts.py
--rw-r--r--   0     1001     1002    52357 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription.py
--rw-r--r--   0     1001     1002    59922 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_async.py
--rw-r--r--   0     1001     1002    31605 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_async_all_of.py
--rw-r--r--   0     1001     1002    50376 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_common.py
--rw-r--r--   0     1001     1002    36485 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_common_lm.py
--rw-r--r--   0     1001     1002    34664 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
--rw-r--r--   0     1001     1002    55626 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_defaults.py
--rw-r--r--   0     1001     1002    51007 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_sa.py
--rw-r--r--   0     1001     1002    31791 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_speakers.py
--rw-r--r--   0     1001     1002    33208 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
--rw-r--r--   0     1001     1002    34411 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/asr_transcribe_queue_status.py
--rw-r--r--   0     1001     1002    34140 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_audio_input_source.py
--rw-r--r--   0     1001     1002    29596 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_mode.py
--rw-r--r--   0     1001     1002    29640 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_mode_recognition.py
--rw-r--r--   0     1001     1002    29557 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_mode_speech_analytics.py
--rw-r--r--   0     1001     1002    29603 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_mode_transcription.py
--rw-r--r--   0     1001     1002    31777 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_post_response_base.py
--rw-r--r--   0     1001     1002    31172 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_post_response_base_audio.py
--rw-r--r--   0     1001     1002    32850 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_reco_post_response.py
--rw-r--r--   0     1001     1002    30527 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_reco_post_response_sessions.py
--rw-r--r--   0     1001     1002    30439 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_callback_response.py
--rw-r--r--   0     1001     1002    32071 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_request.py
--rw-r--r--   0     1001     1002    32201 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_response.py
--rw-r--r--   0     1001     1002    34960 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_result.py
--rw-r--r--   0     1001     1002    30226 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_result_all_of.py
--rw-r--r--   0     1001     1002    33788 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full.py
--rw-r--r--   0     1001     1002    31697 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of.py
--rw-r--r--   0     1001     1002    30899 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio.py
--rw-r--r--   0     1001     1002    37214 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio_callback.py
--rw-r--r--   0     1001     1002    30313 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio_source.py
--rw-r--r--   0     1001     1002    30325 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
--rw-r--r--   0     1001     1002    43658 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_result.py
--rw-r--r--   0     1001     1002    33329 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental.py
--rw-r--r--   0     1001     1002    31146 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail.py
--rw-r--r--   0     1001     1002    31184 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail_control_status.py
--rw-r--r--   0     1001     1002    39939 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail_result.py
--rw-r--r--   0     1001     1002    34455 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
--rw-r--r--   0     1001     1002    33331 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_session_established.py
--rw-r--r--   0     1001     1002    32713 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_session_short_info.py
--rw-r--r--   0     1001     1002    30340 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_session_url.py
--rw-r--r--   0     1001     1002    32908 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transc_post_response.py
--rw-r--r--   0     1001     1002    30561 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transc_post_response_sessions.py
--rw-r--r--   0     1001     1002    35406 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transc_session_established.py
--rw-r--r--   0     1001     1002    30367 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_callback_response.py
--rw-r--r--   0     1001     1002    32008 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_request.py
--rw-r--r--   0     1001     1002    31381 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_response.py
--rw-r--r--   0     1001     1002    31809 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_response_shared.py
--rw-r--r--   0     1001     1002    29560 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_channel.py
--rw-r--r--   0     1001     1002    29538 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_channel_selector.py
--rw-r--r--   0     1001     1002    29631 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_channel_selector_offline_async.py
--rw-r--r--   0     1001     1002    29492 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_channels.py
--rw-r--r--   0     1001     1002    30187 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_for_data_object.py
--rw-r--r--   0     1001     1002    29607 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_format.py
--rw-r--r--   0     1001     1002    34038 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_async.py
--rw-r--r--   0     1001     1002    30253 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_async_source.py
--rw-r--r--   0     1001     1002    35160 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_async_with_callback.py
--rw-r--r--   0     1001     1002    33175 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_base.py
--rw-r--r--   0     1001     1002    30128 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_callback.py
--rw-r--r--   0     1001     1002    35291 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_callback_callback.py
--rw-r--r--   0     1001     1002    29362 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_data.py
--rw-r--r--   0     1001     1002    31544 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_data_all_of.py
--rw-r--r--   0     1001     1002    31444 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_data_all_of_source.py
--rw-r--r--   0     1001     1002    35001 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_sync.py
--rw-r--r--   0     1001     1002    31260 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_input_sync_source.py
--rw-r--r--   0     1001     1002    34472 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_resource_uri.py
--rw-r--r--   0     1001     1002    29592 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_zone_class.py
--rw-r--r--   0     1001     1002    31503 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/audio_zone_item.py
--rw-r--r--   0     1001     1002    30033 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/basic_success_response.py
--rw-r--r--   0     1001     1002    31535 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/builtin.py
--rw-r--r--   0     1001     1002    31595 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/builtin_all_of.py
--rw-r--r--   0     1001     1002    29874 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/call_attributes.py
--rw-r--r--   0     1001     1002    36589 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/call_review_answer_alone.py
--rw-r--r--   0     1001     1002    29523 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/call_review_answer_type.py
--rw-r--r--   0     1001     1002    33995 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/call_review_config_question_base.py
--rw-r--r--   0     1001     1002    43456 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/call_review_config_question_base_with_answer.py
--rw-r--r--   0     1001     1002    35753 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/call_review_config_question_base_with_id.py
--rw-r--r--   0     1001     1002    35242 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/callback_req.py
--rw-r--r--   0     1001     1002    32000 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/callback_req_reco.py
--rw-r--r--   0     1001     1002    30161 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/callback_resp.py
--rw-r--r--   0     1001     1002    33943 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/caption.py
--rw-r--r--   0     1001     1002    31003 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/compliance_settings.py
--rw-r--r--   0     1001     1002    29553 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/config_value_status.py
--rw-r--r--   0     1001     1002    29649 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/content_type.py
--rw-r--r--   0     1001     1002    33070 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/continuous_recognition.py
--rw-r--r--   0     1001     1002    50287 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/core_aivr_session.py
--rw-r--r--   0     1001     1002    39312 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/core_aivr_session_telco_data.py
--rw-r--r--   0     1001     1002    30992 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/cr_question_id_for_cr_config.py
--rw-r--r--   0     1001     1002    29517 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/creating_entity.py
--rw-r--r--   0     1001     1002    31202 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/criterion_config.py
--rw-r--r--   0     1001     1002    31103 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/criterion_satisfied.py
--rw-r--r--   0     1001     1002    30029 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_obj_ref.py
--rw-r--r--   0     1001     1002    44554 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_object.py
--rw-r--r--   0     1001     1002    30023 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_object_all_of.py
--rw-r--r--   0     1001     1002    38551 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_object_base.py
--rw-r--r--   0     1001     1002    34912 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_object_ids.py
--rw-r--r--   0     1001     1002    44333 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_object_no_sos_ref.py
--rw-r--r--   0     1001     1002    39524 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/data_object_with_audio.py
--rw-r--r--   0     1001     1002    29967 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/debug_info.py
--rw-r--r--   0     1001     1002    30573 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/debug_settings.py
--rw-r--r--   0     1001     1002    32572 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/demo.py
--rw-r--r--   0     1001     1002    32652 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/demo_all_of.py
--rw-r--r--   0     1001     1002    30959 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/diarization_data.py
--rw-r--r--   0     1001     1002    30828 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/diarization_zone.py
--rw-r--r--   0     1001     1002    36024 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/diarization_zone_item.py
--rw-r--r--   0     1001     1002    32690 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/disconnect.py
--rw-r--r--   0     1001     1002    32770 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/disconnect_all_of.py
--rw-r--r--   0     1001     1002    31022 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/error.py
--rw-r--r--   0     1001     1002    31082 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/error_all_of.py
--rw-r--r--   0     1001     1002    31070 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/error_info.py
--rw-r--r--   0     1001     1002    31631 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/estimated_queue_wait.py
--rw-r--r--   0     1001     1002    29572 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/experiment_platform.py
--rw-r--r--   0     1001     1002    32045 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/file_location.py
--rw-r--r--   0     1001     1002    35993 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/formatter.py
--rw-r--r--   0     1001     1002    30947 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/grammar.py
--rw-r--r--   0     1001     1002    30254 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg.py
--rw-r--r--   0     1001     1002    30294 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_all_of.py
--rw-r--r--   0     1001     1002    37405 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio.py
--rw-r--r--   0     1001     1002    31270 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_all_of.py
--rw-r--r--   0     1001     1002    32915 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_base.py
--rw-r--r--   0     1001     1002    33920 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_base_with_audio.py
--rw-r--r--   0     1001     1002    30260 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_id.py
--rw-r--r--   0     1001     1002    30912 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input.py
--rw-r--r--   0     1001     1002    30242 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input_audio_hash.py
--rw-r--r--   0     1001     1002    30160 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input_audio_id.py
--rw-r--r--   0     1001     1002    30187 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input_data.py
--rw-r--r--   0     1001     1002    34267 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set.py
--rw-r--r--   0     1001     1002    31590 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_base.py
--rw-r--r--   0     1001     1002    31663 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_base_inclusive.py
--rw-r--r--   0     1001     1002    32503 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_core.py
--rw-r--r--   0     1001     1002    30267 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_id.py
--rw-r--r--   0     1001     1002    32532 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_inclusive.py
--rw-r--r--   0     1001     1002    32612 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_inclusive_core.py
--rw-r--r--   0     1001     1002    32523 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_inner.py
--rw-r--r--   0     1001     1002    31361 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_response.py
--rw-r--r--   0     1001     1002    35729 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_thin.py
--rw-r--r--   0     1001     1002    38873 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment.py
--rw-r--r--   0     1001     1002    36230 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_base.py
--rw-r--r--   0     1001     1002    34966 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_base_inclusive.py
--rw-r--r--   0     1001     1002    31921 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_base_platform_data.py
--rw-r--r--   0     1001     1002    30305 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_id.py
--rw-r--r--   0     1001     1002    37733 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_inclusive.py
--rw-r--r--   0     1001     1002    35904 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_modifiable.py
--rw-r--r--   0     1001     1002    35528 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_platform_external_asr.py
--rw-r--r--   0     1001     1002    30571 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_platform_upload.py
--rw-r--r--   0     1001     1002    31283 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_platform_voicegain.py
--rw-r--r--   0     1001     1002    31389 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_response.py
--rw-r--r--   0     1001     1002    29673 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_status.py
--rw-r--r--   0     1001     1002    29602 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_status_modifiable.py
--rw-r--r--   0     1001     1002    34584 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar.py
--rw-r--r--   0     1001     1002    31856 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_base.py
--rw-r--r--   0     1001     1002    30860 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_base_light.py
--rw-r--r--   0     1001     1002    30322 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_id.py
--rw-r--r--   0     1001     1002    31788 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_inner.py
--rw-r--r--   0     1001     1002    33664 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_light.py
--rw-r--r--   0     1001     1002    30973 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_interpretation.py
--rw-r--r--   0     1001     1002    35203 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_question.py
--rw-r--r--   0     1001     1002    32456 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_question_base.py
--rw-r--r--   0     1001     1002    30353 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_question_id.py
--rw-r--r--   0     1001     1002    33479 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_question_inner.py
--rw-r--r--   0     1001     1002    31199 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
--rw-r--r--   0     1001     1002    33675 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
--rw-r--r--   0     1001     1002    31112 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
--rw-r--r--   0     1001     1002    31042 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
--rw-r--r--   0     1001     1002    30316 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_with_exp.py
--rw-r--r--   0     1001     1002    37165 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recognition.py
--rw-r--r--   0     1001     1002    34457 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recognition_base.py
--rw-r--r--   0     1001     1002    30334 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_recognition_id.py
--rw-r--r--   0     1001     1002    29621 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_review_status.py
--rw-r--r--   0     1001     1002    32584 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_source_of_truth.py
--rw-r--r--   0     1001     1002    33458 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_truth_update.py
--rw-r--r--   0     1001     1002    33218 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/greg_truth_updates.py
--rw-r--r--   0     1001     1002    32203 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/grxml.py
--rw-r--r--   0     1001     1002    32303 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/grxml_all_of.py
--rw-r--r--   0     1001     1002    30712 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/gui_input.py
--rw-r--r--   0     1001     1002    29330 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/hangup.py
--rw-r--r--   0     1001     1002    30002 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/html_checkbox.py
--rw-r--r--   0     1001     1002    31816 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/html_choice_item.py
--rw-r--r--   0     1001     1002    30034 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/html_radio_buttons.py
--rw-r--r--   0     1001     1002    30097 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/html_text_entry.py
--rw-r--r--   0     1001     1002    29490 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/if_exists.py
--rw-r--r--   0     1001     1002    33514 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/incident.py
--rw-r--r--   0     1001     1002    30021 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/inline_data.py
--rw-r--r--   0     1001     1002    31226 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/inline_object.py
--rw-r--r--   0     1001     1002    31238 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/inline_object1.py
--rw-r--r--   0     1001     1002    34641 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/input.py
--rw-r--r--   0     1001     1002    34781 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/input_all_of.py
--rw-r--r--   0     1001     1002    30941 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/integration.py
--rw-r--r--   0     1001     1002    36117 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/jjsgf.py
--rw-r--r--   0     1001     1002    36257 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/jjsgf_all_of.py
--rw-r--r--   0     1001     1002    31408 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/keyword_spot_example.py
--rw-r--r--   0     1001     1002    31393 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/keyword_spot_group.py
--rw-r--r--   0     1001     1002    33136 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/keyword_spot_item.py
--rw-r--r--   0     1001     1002    29614 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/lang_model_status.py
--rw-r--r--   0     1001     1002    30390 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/language.py
--rw-r--r--   0     1001     1002    39717 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/language_model_doc.py
--rw-r--r--   0     1001     1002    38174 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/language_model_doc_modifiable.py
--rw-r--r--   0     1001     1002    32932 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/language_model_src_data.py
--rw-r--r--   0     1001     1002    29491 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/lm_type.py
--rw-r--r--   0     1001     1002    30153 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/min_max_speakers.py
--rw-r--r--   0     1001     1002    32994 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/min_max_speakers_diarization.py
--rw-r--r--   0     1001     1002    29643 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/mood_type.py
--rw-r--r--   0     1001     1002    31486 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/mrc_pv1_asr_settings.py
--rw-r--r--   0     1001     1002    31459 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/mrc_pv2_asr_settings.py
--rw-r--r--   0     1001     1002    29490 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/mrcp_version.py
--rw-r--r--   0     1001     1002    33331 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/multipart_form_data_field.py
--rw-r--r--   0     1001     1002    31973 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/name_value_pair.py
--rw-r--r--   0     1001     1002    30985 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/named_entity_concept.py
--rw-r--r--   0     1001     1002    30106 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/named_entity_type.py
--rw-r--r--   0     1001     1002    49870 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session.py
--rw-r--r--   0     1001     1002    38284 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session_response.py
--rw-r--r--   0     1001     1002    30317 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session_response_poll.py
--rw-r--r--   0     1001     1002    30223 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
--rw-r--r--   0     1001     1002    30871 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/non_session_error_response.py
--rw-r--r--   0     1001     1002    29410 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/non_session_error_response400.py
--rw-r--r--   0     1001     1002    29410 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/non_session_error_response401.py
--rw-r--r--   0     1001     1002    32304 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/output.py
--rw-r--r--   0     1001     1002    32384 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/output_all_of.py
--rw-r--r--   0     1001     1002    34586 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/overtalk.py
--rw-r--r--   0     1001     1002    32778 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phone_audio_input.py
--rw-r--r--   0     1001     1002    30996 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phone_audio_input_prompt.py
--rw-r--r--   0     1001     1002    33627 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_example.py
--rw-r--r--   0     1001     1002    33493 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_group.py
--rw-r--r--   0     1001     1002    41136 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item.py
--rw-r--r--   0     1001     1002    32457 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item_location.py
--rw-r--r--   0     1001     1002    32237 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item_location_dialogue.py
--rw-r--r--   0     1001     1002    31097 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item_slots.py
--rw-r--r--   0     1001     1002    33033 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/pii_redaction_conf.py
--rw-r--r--   0     1001     1002    33835 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/poll_req.py
--rw-r--r--   0     1001     1002    33611 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/poll_resp.py
--rw-r--r--   0     1001     1002    33581 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/portal_output_init.py
--rw-r--r--   0     1001     1002    30370 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/pre_fetch.py
--rw-r--r--   0     1001     1002    41039 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/progress.py
--rw-r--r--   0     1001     1002    31855 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/progress_callback.py
--rw-r--r--   0     1001     1002    29777 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/progress_phase.py
--rw-r--r--   0     1001     1002    32899 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/quartiles_energy.py
--rw-r--r--   0     1001     1002    32875 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/quartiles_pitch.py
--rw-r--r--   0     1001     1002    34684 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/reco_alt.py
--rw-r--r--   0     1001     1002    31885 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/recog_nlsml.py
--rw-r--r--   0     1001     1002    31055 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/recog_nlsml_no_exp.py
--rw-r--r--   0     1001     1002    34149 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/recog_obj.py
--rw-r--r--   0     1001     1002    33387 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/recog_obj_no_exp.py
--rw-r--r--   0     1001     1002    34048 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/recognition_result.py
--rw-r--r--   0     1001     1002    34317 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/requested_content.py
--rw-r--r--   0     1001     1002    33328 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/resource_uri.py
--rw-r--r--   0     1001     1002    29580 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/results_websocket_mode.py
--rw-r--r--   0     1001     1002    35227 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/s3.py
--rw-r--r--   0     1001     1002    35387 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/s3_all_of.py
--rw-r--r--   0     1001     1002    35344 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/s3_audio_input.py
--rw-r--r--   0     1001     1002    31595 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/s3_metadata_mapping.py
--rw-r--r--   0     1001     1002    31373 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/s3_tag_mapping.py
--rw-r--r--   0     1001     1002    29507 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sa_conf_type.py
--rw-r--r--   0     1001     1002    29626 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sample_rate.py
--rw-r--r--   0     1001     1002    35578 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sentence_hypothesis_or_recognition.py
--rw-r--r--   0     1001     1002    31913 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py
--rw-r--r--   0     1001     1002    34035 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sentence_recognition.py
--rw-r--r--   0     1001     1002    30203 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/session_content.py
--rw-r--r--   0     1001     1002    31715 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/session_error_response.py
--rw-r--r--   0     1001     1002    37731 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/session_init_recognition.py
--rw-r--r--   0     1001     1002    39973 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/session_init_transcription.py
--rw-r--r--   0     1001     1002    33135 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/session_init_transcription_diarization.py
--rw-r--r--   0     1001     1002    30937 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/session_success_response.py
--rw-r--r--   0     1001     1002    35546 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/settings_async_transcription.py
--rw-r--r--   0     1001     1002    32467 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/settings_recognition.py
--rw-r--r--   0     1001     1002    32440 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/settings_sync_transcription.py
--rw-r--r--   0     1001     1002    34452 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/silence.py
--rw-r--r--   0     1001     1002    31098 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/slot_entity.py
--rw-r--r--   0     1001     1002    31045 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/slot_keyword.py
--rw-r--r--   0     1001     1002    31132 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sos_ref.py
--rw-r--r--   0     1001     1002    33791 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speaker_result.py
--rw-r--r--   0     1001     1002    44599 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_base_result.py
--rw-r--r--   0     1001     1002    32274 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_channel.py
--rw-r--r--   0     1001     1002    45972 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_channel_result.py
--rw-r--r--   0     1001     1002    34258 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
--rw-r--r--   0     1001     1002    71030 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config.py
--rw-r--r--   0     1001     1002    34716 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_identifying.py
--rw-r--r--   0     1001     1002    68305 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_modifiable.py
--rw-r--r--   0     1001     1002    67025 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_modifiable_base.py
--rw-r--r--   0     1001     1002    31583 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
--rw-r--r--   0     1001     1002    31126 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_name_optional.py
--rw-r--r--   0     1001     1002    31280 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_name_required.py
--rw-r--r--   0     1001     1002    50326 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_core_result.py
--rw-r--r--   0     1001     1002    35253 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_core_result_all_of.py
--rw-r--r--   0     1001     1002    31192 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_criteria_data.py
--rw-r--r--   0     1001     1002    31657 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_emotion.py
--rw-r--r--   0     1001     1002    30860 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_emotion_data.py
--rw-r--r--   0     1001     1002    36981 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_emotion_item.py
--rw-r--r--   0     1001     1002    30906 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword.py
--rw-r--r--   0     1001     1002    31196 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_data.py
--rw-r--r--   0     1001     1002    36230 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_item.py
--rw-r--r--   0     1001     1002    36482 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
--rw-r--r--   0     1001     1002    32744 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py
--rw-r--r--   0     1001     1002    31876 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity.py
--rw-r--r--   0     1001     1002    37280 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity_item.py
--rw-r--r--   0     1001     1002    37568 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
--rw-r--r--   0     1001     1002    33818 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py
--rw-r--r--   0     1001     1002    32962 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase.py
--rw-r--r--   0     1001     1002    31179 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_data.py
--rw-r--r--   0     1001     1002    33077 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_for_ws.py
--rw-r--r--   0     1001     1002    31166 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py
--rw-r--r--   0     1001     1002    31005 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group.py
--rw-r--r--   0     1001     1002    31278 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group_data.py
--rw-r--r--   0     1001     1002    31038 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py
--rw-r--r--   0     1001     1002    36393 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group_item.py
--rw-r--r--   0     1001     1002    38302 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_item.py
--rw-r--r--   0     1001     1002    39702 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
--rw-r--r--   0     1001     1002    31076 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_slots.py
--rw-r--r--   0     1001     1002    61306 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_result.py
--rw-r--r--   0     1001     1002    46633 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_result_detail.py
--rw-r--r--   0     1001     1002    31091 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_session_modifiable.py
--rw-r--r--   0     1001     1002    38026 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_session_poll_response.py
--rw-r--r--   0     1001     1002    36321 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_websocket_payload.py
--rw-r--r--   0     1001     1002    31728 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/start_end_time_for_sub_criterion.py
--rw-r--r--   0     1001     1002    30414 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stomp_ping.py
--rw-r--r--   0     1001     1002    33034 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stomp_word_correction.py
--rw-r--r--   0     1001     1002    37053 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stomp_ws_word.py
--rw-r--r--   0     1001     1002    31191 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stomp_ws_word_all_of.py
--rw-r--r--   0     1001     1002    35348 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stomp_ws_word_base.py
--rw-r--r--   0     1001     1002    35620 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stream_resp.py
--rw-r--r--   0     1001     1002    33181 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/stream_setup.py
--rw-r--r--   0     1001     1002    29634 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/streaming_protocol.py
--rw-r--r--   0     1001     1002    38813 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sub_criterion_config.py
--rw-r--r--   0     1001     1002    41199 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sub_criterion_satisfied.py
--rw-r--r--   0     1001     1002    32174 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_audio_input_source.py
--rw-r--r--   0     1001     1002    31122 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_recognition_request.py
--rw-r--r--   0     1001     1002    32687 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_recognition_response.py
--rw-r--r--   0     1001     1002    30290 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_session_established.py
--rw-r--r--   0     1001     1002    31006 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_transcription_request.py
--rw-r--r--   0     1001     1002    32745 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_transcription_response.py
--rw-r--r--   0     1001     1002    33184 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/sync_transcription_result.py
--rw-r--r--   0     1001     1002    38900 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/talk_time.py
--rw-r--r--   0     1001     1002    31431 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/topic_score.py
--rw-r--r--   0     1001     1002    29530 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_bucket_type.py
--rw-r--r--   0     1001     1002    39172 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_doc.py
--rw-r--r--   0     1001     1002    31090 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_doc_defaults.py
--rw-r--r--   0     1001     1002    36550 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_doc_statistics.py
--rw-r--r--   0     1001     1002    34624 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_key.py
--rw-r--r--   0     1001     1002    33874 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_modifiable.py
--rw-r--r--   0     1001     1002    29622 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_status.py
--rw-r--r--   0     1001     1002    29662 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_status_modifiable.py
--rw-r--r--   0     1001     1002    29550 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/training_set_store_type.py
--rw-r--r--   0     1001     1002    31792 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcribe_alt.py
--rw-r--r--   0     1001     1002    31074 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_id.py
--rw-r--r--   0     1001     1002    34092 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_modify_request.py
--rw-r--r--   0     1001     1002    31769 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_modify_request_mute.py
--rw-r--r--   0     1001     1002    30597 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_modify_request_pause.py
--rw-r--r--   0     1001     1002    34626 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcript_position_range.py
--rw-r--r--   0     1001     1002    34806 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcript_position_range_for_phrase.py
--rw-r--r--   0     1001     1002    36042 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
--rw-r--r--   0     1001     1002    36363 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transfer.py
--rw-r--r--   0     1001     1002    36503 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/transfer_all_of.py
--rw-r--r--   0     1001     1002    29546 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/vad_mode.py
--rw-r--r--   0     1001     1002    32351 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/version.py
--rw-r--r--   0     1001     1002    38003 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket.py
--rw-r--r--   0     1001     1002    41057 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket_init.py
--rw-r--r--   0     1001     1002    30564 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket_init_reco.py
--rw-r--r--   0     1001     1002    36159 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket_modifiable.py
--rw-r--r--   0     1001     1002    32627 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket_msg.py
--rw-r--r--   0     1001     1002    29493 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket_protocol.py
--rw-r--r--   0     1001     1002    30968 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/websocket_resp.py
--rw-r--r--   0     1001     1002    30325 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_alternatives.py
--rw-r--r--   0     1001     1002    31505 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_cloud_item.py
--rw-r--r--   0     1001     1002    31346 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_correction.py
--rw-r--r--   0     1001     1002    36356 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_item_timed.py
--rw-r--r--   0     1001     1002    31431 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_item_timing.py
--rw-r--r--   0     1001     1002    30686 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_tree_ids.py
--rw-r--r--   0     1001     1002    36733 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/word_tree_item.py
--rw-r--r--   0     1001     1002    33288 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_item.py
--rw-r--r--   0     1001     1002    36591 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_section.py
--rw-r--r--   0     1001     1002    33137 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_section_meta.py
--rw-r--r--   0     1001     1002    32139 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_section_meta_mc.py
--rw-r--r--   0     1001     1002    34118 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_section_single_column.py
--rw-r--r--   0     1001     1002    30199 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_section_words.py
--rw-r--r--   0     1001     1002    44224 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/words_websocket_item.py
--rw-r--r--   0     1001     1002    33875 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_emotion_item.py
--rw-r--r--   0     1001     1002    33124 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_keyword_item.py
--rw-r--r--   0     1001     1002    34114 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_named_entity_item.py
--rw-r--r--   0     1001     1002    32348 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_phrase_group_item.py
--rw-r--r--   0     1001     1002    35127 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_phrase_item.py
--rw-r--r--   0     1001     1002    35479 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_phrase_item_inside_group.py
--rw-r--r--   0     1001     1002    31700 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_position_range.py
--rw-r--r--   0     1001     1002    30884 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_position_range_nested.py
--rw-r--r--   0     1001     1002    30872 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_position_range_no_spk.py
--rw-r--r--   0     1001     1002    37497 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py
--rw-r--r--   0     1001     1002    31349 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py
--rw-r--r--   0     1001     1002    32682 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_speaker.py
--rw-r--r--   0     1001     1002    34542 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_word.py
--rw-r--r--   0     1001     1002    32108 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/models/ws_word_edit.py
--rw-r--r--   0     1001     1002    39169 2023-06-29 21:55:26.000000 voicegain-speech-1.85.1/voicegain_speech/rest.py
-drwxr-xr-x   0     1001     1002        0 2023-06-29 21:55:29.012389 voicegain-speech-1.85.1/voicegain_speech.egg-info/
--rw-r--r--   0     1001     1002     2923 2023-06-29 21:55:28.000000 voicegain-speech-1.85.1/voicegain_speech.egg-info/PKG-INFO
--rw-r--r--   0     1001     1002    22939 2023-06-29 21:55:28.000000 voicegain-speech-1.85.1/voicegain_speech.egg-info/SOURCES.txt
--rw-r--r--   0     1001     1002        1 2023-06-29 21:55:28.000000 voicegain-speech-1.85.1/voicegain_speech.egg-info/dependency_links.txt
--rw-r--r--   0     1001     1002       48 2023-06-29 21:55:28.000000 voicegain-speech-1.85.1/voicegain_speech.egg-info/requires.txt
--rw-r--r--   0     1001     1002       17 2023-06-29 21:55:28.000000 voicegain-speech-1.85.1/voicegain_speech.egg-info/top_level.txt
+drwxr-xr-x   0     1001     1002        0 2023-06-30 03:38:40.325347 voicegain-speech-1.85.2/
+-rw-r--r--   0     1001     1002    11357 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/LICENSE
+-rw-r--r--   0     1001     1002     2923 2023-06-30 03:38:40.325347 voicegain-speech-1.85.2/PKG-INFO
+-rw-r--r--   0     1001     1002     2491 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/README.md
+-rw-r--r--   0     1001     1002       79 2023-06-30 03:38:40.325347 voicegain-speech-1.85.2/setup.cfg
+-rw-r--r--   0     1001     1002      709 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/setup.py
+drwxr-xr-x   0     1001     1002        0 2023-06-30 03:38:40.201336 voicegain-speech-1.85.2/voicegain_speech/
+-rw-r--r--   0     1001     1002    63205 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/__init__.py
+drwxr-xr-x   0     1001     1002        0 2023-06-30 03:38:40.209337 voicegain-speech-1.85.2/voicegain_speech/api/
+-rw-r--r--   0     1001     1002      821 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/__init__.py
+-rw-r--r--   0     1001     1002    33296 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/aivr_api.py
+-rw-r--r--   0     1001     1002    52231 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/aivr_callback_api.py
+-rw-r--r--   0     1001     1002    39239 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/asr_callback_api.py
+-rw-r--r--   0     1001     1002    34611 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/audiocodes_api.py
+-rw-r--r--   0     1001     1002   107541 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/data_api.py
+-rw-r--r--   0     1001     1002   143654 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/greg_api.py
+-rw-r--r--   0     1001     1002    63228 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/lm_api.py
+-rw-r--r--   0     1001     1002    48177 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/recognize_api.py
+-rw-r--r--   0     1001     1002   118990 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/sa_api.py
+-rw-r--r--   0     1001     1002    37190 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/security_api.py
+-rw-r--r--   0     1001     1002    57369 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/training_api.py
+-rw-r--r--   0     1001     1002   103246 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/transcribe_api.py
+-rw-r--r--   0     1001     1002    55744 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api/websocket_api.py
+-rw-r--r--   0     1001     1002    51954 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/api_client.py
+-rw-r--r--   0     1001     1002    38411 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/configuration.py
+-rw-r--r--   0     1001     1002    30458 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/exceptions.py
+drwxr-xr-x   0     1001     1002        0 2023-06-30 03:38:40.325347 voicegain-speech-1.85.2/voicegain_speech/models/
+-rw-r--r--   0     1001     1002    62021 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/__init__.py
+-rw-r--r--   0     1001     1002    40147 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_control_messages.py
+-rw-r--r--   0     1001     1002    31410 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_end.py
+-rw-r--r--   0     1001     1002    31418 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_error.py
+-rw-r--r--   0     1001     1002    31536 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_hypothesis.py
+-rw-r--r--   0     1001     1002    30265 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_hypothesis_alternatives.py
+-rw-r--r--   0     1001     1002    31506 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_recognition.py
+-rw-r--r--   0     1001     1002    31669 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_recognition_alternatives.py
+-rw-r--r--   0     1001     1002    32543 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_response_messages.py
+-rw-r--r--   0     1001     1002    39630 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_start.py
+-rw-r--r--   0     1001     1002    31682 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_start_stt_speech_contexts.py
+-rw-r--r--   0     1001     1002    30535 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_started.py
+-rw-r--r--   0     1001     1002    30604 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ac_stop.py
+-rw-r--r--   0     1001     1002    31282 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/account_and_context_id.py
+-rw-r--r--   0     1001     1002    34185 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/advanced_regex.py
+-rw-r--r--   0     1001     1002    30212 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aircall.py
+-rw-r--r--   0     1001     1002    30252 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aircall_all_of.py
+-rw-r--r--   0     1001     1002    36151 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_callback_response.py
+-rw-r--r--   0     1001     1002    31567 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_callback_response_final.py
+-rw-r--r--   0     1001     1002    30229 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_conference_transfer.py
+-rw-r--r--   0     1001     1002    30887 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_disconnect.py
+-rw-r--r--   0     1001     1002    33825 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_event.py
+-rw-r--r--   0     1001     1002    29630 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_event_type.py
+-rw-r--r--   0     1001     1002    33088 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_existing_session.py
+-rw-r--r--   0     1001     1002    32700 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic.py
+-rw-r--r--   0     1001     1002    29493 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic_media.py
+-rw-r--r--   0     1001     1002    31442 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic_transfer.py
+-rw-r--r--   0     1001     1002    29579 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic_type.py
+-rw-r--r--   0     1001     1002    41441 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_new_session.py
+-rw-r--r--   0     1001     1002    30984 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_phone_transfer.py
+-rw-r--r--   0     1001     1002    33974 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt.py
+-rw-r--r--   0     1001     1002    30671 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_completion.py
+-rw-r--r--   0     1001     1002    35387 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_playing.py
+-rw-r--r--   0     1001     1002    30195 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_properties_audio.py
+-rw-r--r--   0     1001     1002    30205 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_properties_html.py
+-rw-r--r--   0     1001     1002    36852 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_question.py
+-rw-r--r--   0     1001     1002    29590 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_recognition_result.py
+-rw-r--r--   0     1001     1002    35657 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_recording.py
+-rw-r--r--   0     1001     1002    41835 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_response_properties_audio.py
+-rw-r--r--   0     1001     1002    31782 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_response_properties_html.py
+-rw-r--r--   0     1001     1002    34452 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_session_user.py
+-rw-r--r--   0     1001     1002    30558 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_session_user_base.py
+-rw-r--r--   0     1001     1002    33324 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_session_user_fs.py
+-rw-r--r--   0     1001     1002    32024 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivr_transfer.py
+-rw-r--r--   0     1001     1002    32352 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/aivrs_question_specifics.py
+-rw-r--r--   0     1001     1002    31632 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/answer_map_entry.py
+-rw-r--r--   0     1001     1002    29584 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_event.py
+-rw-r--r--   0     1001     1002    29675 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status.py
+-rw-r--r--   0     1001     1002    29595 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status_additional.py
+-rw-r--r--   0     1001     1002    29650 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status_after_input_started.py
+-rw-r--r--   0     1001     1002    29677 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status_for_callback.py
+-rw-r--r--   0     1001     1002    29586 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_recognition_result.py
+-rw-r--r--   0     1001     1002    42889 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_common.py
+-rw-r--r--   0     1001     1002    56905 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition.py
+-rw-r--r--   0     1001     1002    52269 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition_defaults.py
+-rw-r--r--   0     1001     1002    43582 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
+-rw-r--r--   0     1001     1002    38338 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition_timeouts.py
+-rw-r--r--   0     1001     1002    52357 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription.py
+-rw-r--r--   0     1001     1002    59922 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_async.py
+-rw-r--r--   0     1001     1002    31605 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_async_all_of.py
+-rw-r--r--   0     1001     1002    50376 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_common.py
+-rw-r--r--   0     1001     1002    36485 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_common_lm.py
+-rw-r--r--   0     1001     1002    34664 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
+-rw-r--r--   0     1001     1002    55626 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_defaults.py
+-rw-r--r--   0     1001     1002    51007 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_sa.py
+-rw-r--r--   0     1001     1002    31791 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_speakers.py
+-rw-r--r--   0     1001     1002    33208 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
+-rw-r--r--   0     1001     1002    34411 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/asr_transcribe_queue_status.py
+-rw-r--r--   0     1001     1002    34140 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_audio_input_source.py
+-rw-r--r--   0     1001     1002    29596 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_mode.py
+-rw-r--r--   0     1001     1002    29640 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_mode_recognition.py
+-rw-r--r--   0     1001     1002    29557 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_mode_speech_analytics.py
+-rw-r--r--   0     1001     1002    29603 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_mode_transcription.py
+-rw-r--r--   0     1001     1002    31777 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_post_response_base.py
+-rw-r--r--   0     1001     1002    31172 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_post_response_base_audio.py
+-rw-r--r--   0     1001     1002    32850 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_reco_post_response.py
+-rw-r--r--   0     1001     1002    30527 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_reco_post_response_sessions.py
+-rw-r--r--   0     1001     1002    30439 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_callback_response.py
+-rw-r--r--   0     1001     1002    32071 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_request.py
+-rw-r--r--   0     1001     1002    32201 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_response.py
+-rw-r--r--   0     1001     1002    34960 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_result.py
+-rw-r--r--   0     1001     1002    30226 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_result_all_of.py
+-rw-r--r--   0     1001     1002    33788 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full.py
+-rw-r--r--   0     1001     1002    31697 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of.py
+-rw-r--r--   0     1001     1002    30899 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio.py
+-rw-r--r--   0     1001     1002    37214 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio_callback.py
+-rw-r--r--   0     1001     1002    30313 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio_source.py
+-rw-r--r--   0     1001     1002    30325 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
+-rw-r--r--   0     1001     1002    43658 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_result.py
+-rw-r--r--   0     1001     1002    33329 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental.py
+-rw-r--r--   0     1001     1002    31146 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail.py
+-rw-r--r--   0     1001     1002    31184 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail_control_status.py
+-rw-r--r--   0     1001     1002    39939 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail_result.py
+-rw-r--r--   0     1001     1002    34455 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
+-rw-r--r--   0     1001     1002    33331 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_session_established.py
+-rw-r--r--   0     1001     1002    32713 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_session_short_info.py
+-rw-r--r--   0     1001     1002    30340 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_session_url.py
+-rw-r--r--   0     1001     1002    32908 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transc_post_response.py
+-rw-r--r--   0     1001     1002    30561 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transc_post_response_sessions.py
+-rw-r--r--   0     1001     1002    35406 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transc_session_established.py
+-rw-r--r--   0     1001     1002    30367 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_callback_response.py
+-rw-r--r--   0     1001     1002    32008 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_request.py
+-rw-r--r--   0     1001     1002    31381 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_response.py
+-rw-r--r--   0     1001     1002    31809 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_response_shared.py
+-rw-r--r--   0     1001     1002    29560 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_channel.py
+-rw-r--r--   0     1001     1002    29538 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_channel_selector.py
+-rw-r--r--   0     1001     1002    29631 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_channel_selector_offline_async.py
+-rw-r--r--   0     1001     1002    29492 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_channels.py
+-rw-r--r--   0     1001     1002    30187 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_for_data_object.py
+-rw-r--r--   0     1001     1002    29607 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_format.py
+-rw-r--r--   0     1001     1002    34038 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_async.py
+-rw-r--r--   0     1001     1002    30253 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_async_source.py
+-rw-r--r--   0     1001     1002    35160 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_async_with_callback.py
+-rw-r--r--   0     1001     1002    33175 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_base.py
+-rw-r--r--   0     1001     1002    30128 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_callback.py
+-rw-r--r--   0     1001     1002    35291 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_callback_callback.py
+-rw-r--r--   0     1001     1002    29362 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_data.py
+-rw-r--r--   0     1001     1002    31544 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_data_all_of.py
+-rw-r--r--   0     1001     1002    31444 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_data_all_of_source.py
+-rw-r--r--   0     1001     1002    35001 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_sync.py
+-rw-r--r--   0     1001     1002    31260 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_input_sync_source.py
+-rw-r--r--   0     1001     1002    34472 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_resource_uri.py
+-rw-r--r--   0     1001     1002    29592 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_zone_class.py
+-rw-r--r--   0     1001     1002    31503 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/audio_zone_item.py
+-rw-r--r--   0     1001     1002    30033 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/basic_success_response.py
+-rw-r--r--   0     1001     1002    31535 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/builtin.py
+-rw-r--r--   0     1001     1002    31595 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/builtin_all_of.py
+-rw-r--r--   0     1001     1002    29874 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/call_attributes.py
+-rw-r--r--   0     1001     1002    36589 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/call_review_answer_alone.py
+-rw-r--r--   0     1001     1002    29523 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/call_review_answer_type.py
+-rw-r--r--   0     1001     1002    33995 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/call_review_config_question_base.py
+-rw-r--r--   0     1001     1002    43456 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/call_review_config_question_base_with_answer.py
+-rw-r--r--   0     1001     1002    35753 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/call_review_config_question_base_with_id.py
+-rw-r--r--   0     1001     1002    35242 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/callback_req.py
+-rw-r--r--   0     1001     1002    32000 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/callback_req_reco.py
+-rw-r--r--   0     1001     1002    30161 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/callback_resp.py
+-rw-r--r--   0     1001     1002    33943 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/caption.py
+-rw-r--r--   0     1001     1002    31003 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/compliance_settings.py
+-rw-r--r--   0     1001     1002    29553 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/config_value_status.py
+-rw-r--r--   0     1001     1002    29649 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/content_type.py
+-rw-r--r--   0     1001     1002    33070 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/continuous_recognition.py
+-rw-r--r--   0     1001     1002    50287 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/core_aivr_session.py
+-rw-r--r--   0     1001     1002    39312 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/core_aivr_session_telco_data.py
+-rw-r--r--   0     1001     1002    30992 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/cr_question_id_for_cr_config.py
+-rw-r--r--   0     1001     1002    29517 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/creating_entity.py
+-rw-r--r--   0     1001     1002    31202 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/criterion_config.py
+-rw-r--r--   0     1001     1002    31103 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/criterion_satisfied.py
+-rw-r--r--   0     1001     1002    30029 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_obj_ref.py
+-rw-r--r--   0     1001     1002    44554 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_object.py
+-rw-r--r--   0     1001     1002    30023 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_object_all_of.py
+-rw-r--r--   0     1001     1002    38551 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_object_base.py
+-rw-r--r--   0     1001     1002    34912 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_object_ids.py
+-rw-r--r--   0     1001     1002    44333 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_object_no_sos_ref.py
+-rw-r--r--   0     1001     1002    39524 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/data_object_with_audio.py
+-rw-r--r--   0     1001     1002    29967 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/debug_info.py
+-rw-r--r--   0     1001     1002    30573 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/debug_settings.py
+-rw-r--r--   0     1001     1002    32572 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/demo.py
+-rw-r--r--   0     1001     1002    32652 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/demo_all_of.py
+-rw-r--r--   0     1001     1002    30959 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/diarization_data.py
+-rw-r--r--   0     1001     1002    30828 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/diarization_zone.py
+-rw-r--r--   0     1001     1002    36024 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/diarization_zone_item.py
+-rw-r--r--   0     1001     1002    32690 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/disconnect.py
+-rw-r--r--   0     1001     1002    32770 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/disconnect_all_of.py
+-rw-r--r--   0     1001     1002    31022 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/error.py
+-rw-r--r--   0     1001     1002    31082 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/error_all_of.py
+-rw-r--r--   0     1001     1002    31070 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/error_info.py
+-rw-r--r--   0     1001     1002    31631 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/estimated_queue_wait.py
+-rw-r--r--   0     1001     1002    29572 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/experiment_platform.py
+-rw-r--r--   0     1001     1002    32045 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/file_location.py
+-rw-r--r--   0     1001     1002    35993 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/formatter.py
+-rw-r--r--   0     1001     1002    30947 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/grammar.py
+-rw-r--r--   0     1001     1002    30254 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg.py
+-rw-r--r--   0     1001     1002    30294 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_all_of.py
+-rw-r--r--   0     1001     1002    37405 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio.py
+-rw-r--r--   0     1001     1002    31270 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_all_of.py
+-rw-r--r--   0     1001     1002    32915 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_base.py
+-rw-r--r--   0     1001     1002    33920 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_base_with_audio.py
+-rw-r--r--   0     1001     1002    30260 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_id.py
+-rw-r--r--   0     1001     1002    30912 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input.py
+-rw-r--r--   0     1001     1002    30242 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input_audio_hash.py
+-rw-r--r--   0     1001     1002    30160 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input_audio_id.py
+-rw-r--r--   0     1001     1002    30187 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input_data.py
+-rw-r--r--   0     1001     1002    34267 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set.py
+-rw-r--r--   0     1001     1002    31590 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_base.py
+-rw-r--r--   0     1001     1002    31663 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_base_inclusive.py
+-rw-r--r--   0     1001     1002    32503 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_core.py
+-rw-r--r--   0     1001     1002    30267 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_id.py
+-rw-r--r--   0     1001     1002    32532 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_inclusive.py
+-rw-r--r--   0     1001     1002    32612 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_inclusive_core.py
+-rw-r--r--   0     1001     1002    32523 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_inner.py
+-rw-r--r--   0     1001     1002    31361 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_response.py
+-rw-r--r--   0     1001     1002    35729 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_thin.py
+-rw-r--r--   0     1001     1002    38873 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment.py
+-rw-r--r--   0     1001     1002    36230 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_base.py
+-rw-r--r--   0     1001     1002    34966 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_base_inclusive.py
+-rw-r--r--   0     1001     1002    31921 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_base_platform_data.py
+-rw-r--r--   0     1001     1002    30305 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_id.py
+-rw-r--r--   0     1001     1002    37733 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_inclusive.py
+-rw-r--r--   0     1001     1002    35904 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_modifiable.py
+-rw-r--r--   0     1001     1002    35528 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_platform_external_asr.py
+-rw-r--r--   0     1001     1002    30571 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_platform_upload.py
+-rw-r--r--   0     1001     1002    31283 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_platform_voicegain.py
+-rw-r--r--   0     1001     1002    31389 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_response.py
+-rw-r--r--   0     1001     1002    29673 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_status.py
+-rw-r--r--   0     1001     1002    29602 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_status_modifiable.py
+-rw-r--r--   0     1001     1002    34584 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar.py
+-rw-r--r--   0     1001     1002    31856 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_base.py
+-rw-r--r--   0     1001     1002    30860 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_base_light.py
+-rw-r--r--   0     1001     1002    30322 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_id.py
+-rw-r--r--   0     1001     1002    31788 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_inner.py
+-rw-r--r--   0     1001     1002    33664 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_light.py
+-rw-r--r--   0     1001     1002    30973 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_interpretation.py
+-rw-r--r--   0     1001     1002    35203 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_question.py
+-rw-r--r--   0     1001     1002    32456 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_question_base.py
+-rw-r--r--   0     1001     1002    30353 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_question_id.py
+-rw-r--r--   0     1001     1002    33479 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_question_inner.py
+-rw-r--r--   0     1001     1002    31199 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
+-rw-r--r--   0     1001     1002    33675 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
+-rw-r--r--   0     1001     1002    31112 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
+-rw-r--r--   0     1001     1002    31042 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
+-rw-r--r--   0     1001     1002    30316 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_with_exp.py
+-rw-r--r--   0     1001     1002    37165 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recognition.py
+-rw-r--r--   0     1001     1002    34457 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recognition_base.py
+-rw-r--r--   0     1001     1002    30334 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_recognition_id.py
+-rw-r--r--   0     1001     1002    29621 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_review_status.py
+-rw-r--r--   0     1001     1002    32584 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_source_of_truth.py
+-rw-r--r--   0     1001     1002    33458 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_truth_update.py
+-rw-r--r--   0     1001     1002    33218 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/greg_truth_updates.py
+-rw-r--r--   0     1001     1002    32203 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/grxml.py
+-rw-r--r--   0     1001     1002    32303 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/grxml_all_of.py
+-rw-r--r--   0     1001     1002    30712 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/gui_input.py
+-rw-r--r--   0     1001     1002    29330 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/hangup.py
+-rw-r--r--   0     1001     1002    30002 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/html_checkbox.py
+-rw-r--r--   0     1001     1002    31816 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/html_choice_item.py
+-rw-r--r--   0     1001     1002    30034 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/html_radio_buttons.py
+-rw-r--r--   0     1001     1002    30097 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/html_text_entry.py
+-rw-r--r--   0     1001     1002    29490 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/if_exists.py
+-rw-r--r--   0     1001     1002    33514 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/incident.py
+-rw-r--r--   0     1001     1002    30021 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/inline_data.py
+-rw-r--r--   0     1001     1002    31226 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/inline_object.py
+-rw-r--r--   0     1001     1002    31238 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/inline_object1.py
+-rw-r--r--   0     1001     1002    34641 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/input.py
+-rw-r--r--   0     1001     1002    34781 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/input_all_of.py
+-rw-r--r--   0     1001     1002    30941 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/integration.py
+-rw-r--r--   0     1001     1002    36117 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/jjsgf.py
+-rw-r--r--   0     1001     1002    36257 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/jjsgf_all_of.py
+-rw-r--r--   0     1001     1002    31408 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/keyword_spot_example.py
+-rw-r--r--   0     1001     1002    31393 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/keyword_spot_group.py
+-rw-r--r--   0     1001     1002    33136 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/keyword_spot_item.py
+-rw-r--r--   0     1001     1002    29614 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/lang_model_status.py
+-rw-r--r--   0     1001     1002    30390 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/language.py
+-rw-r--r--   0     1001     1002    39717 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/language_model_doc.py
+-rw-r--r--   0     1001     1002    38174 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/language_model_doc_modifiable.py
+-rw-r--r--   0     1001     1002    32932 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/language_model_src_data.py
+-rw-r--r--   0     1001     1002    29491 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/lm_type.py
+-rw-r--r--   0     1001     1002    30153 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/min_max_speakers.py
+-rw-r--r--   0     1001     1002    32994 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/min_max_speakers_diarization.py
+-rw-r--r--   0     1001     1002    29643 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/mood_type.py
+-rw-r--r--   0     1001     1002    31486 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/mrc_pv1_asr_settings.py
+-rw-r--r--   0     1001     1002    31459 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/mrc_pv2_asr_settings.py
+-rw-r--r--   0     1001     1002    29490 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/mrcp_version.py
+-rw-r--r--   0     1001     1002    33331 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/multipart_form_data_field.py
+-rw-r--r--   0     1001     1002    31973 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/name_value_pair.py
+-rw-r--r--   0     1001     1002    30985 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/named_entity_concept.py
+-rw-r--r--   0     1001     1002    30106 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/named_entity_type.py
+-rw-r--r--   0     1001     1002    49870 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session.py
+-rw-r--r--   0     1001     1002    38284 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session_response.py
+-rw-r--r--   0     1001     1002    30317 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session_response_poll.py
+-rw-r--r--   0     1001     1002    30223 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
+-rw-r--r--   0     1001     1002    30871 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/non_session_error_response.py
+-rw-r--r--   0     1001     1002    29410 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/non_session_error_response400.py
+-rw-r--r--   0     1001     1002    29410 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/non_session_error_response401.py
+-rw-r--r--   0     1001     1002    32304 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/output.py
+-rw-r--r--   0     1001     1002    32384 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/output_all_of.py
+-rw-r--r--   0     1001     1002    34586 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/overtalk.py
+-rw-r--r--   0     1001     1002    32778 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phone_audio_input.py
+-rw-r--r--   0     1001     1002    30996 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phone_audio_input_prompt.py
+-rw-r--r--   0     1001     1002    33627 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_example.py
+-rw-r--r--   0     1001     1002    33493 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_group.py
+-rw-r--r--   0     1001     1002    41136 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item.py
+-rw-r--r--   0     1001     1002    32457 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item_location.py
+-rw-r--r--   0     1001     1002    32237 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item_location_dialogue.py
+-rw-r--r--   0     1001     1002    31097 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item_slots.py
+-rw-r--r--   0     1001     1002    33033 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/pii_redaction_conf.py
+-rw-r--r--   0     1001     1002    33835 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/poll_req.py
+-rw-r--r--   0     1001     1002    33611 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/poll_resp.py
+-rw-r--r--   0     1001     1002    33581 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/portal_output_init.py
+-rw-r--r--   0     1001     1002    30370 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/pre_fetch.py
+-rw-r--r--   0     1001     1002    41039 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/progress.py
+-rw-r--r--   0     1001     1002    31855 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/progress_callback.py
+-rw-r--r--   0     1001     1002    29777 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/progress_phase.py
+-rw-r--r--   0     1001     1002    32899 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/quartiles_energy.py
+-rw-r--r--   0     1001     1002    32875 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/quartiles_pitch.py
+-rw-r--r--   0     1001     1002    34684 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/reco_alt.py
+-rw-r--r--   0     1001     1002    31885 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/recog_nlsml.py
+-rw-r--r--   0     1001     1002    31055 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/recog_nlsml_no_exp.py
+-rw-r--r--   0     1001     1002    34149 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/recog_obj.py
+-rw-r--r--   0     1001     1002    33387 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/recog_obj_no_exp.py
+-rw-r--r--   0     1001     1002    34048 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/recognition_result.py
+-rw-r--r--   0     1001     1002    34317 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/requested_content.py
+-rw-r--r--   0     1001     1002    33328 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/resource_uri.py
+-rw-r--r--   0     1001     1002    29580 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/results_websocket_mode.py
+-rw-r--r--   0     1001     1002    35227 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/s3.py
+-rw-r--r--   0     1001     1002    35387 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/s3_all_of.py
+-rw-r--r--   0     1001     1002    35344 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/s3_audio_input.py
+-rw-r--r--   0     1001     1002    31595 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/s3_metadata_mapping.py
+-rw-r--r--   0     1001     1002    31373 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/s3_tag_mapping.py
+-rw-r--r--   0     1001     1002    29507 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sa_conf_type.py
+-rw-r--r--   0     1001     1002    29626 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sample_rate.py
+-rw-r--r--   0     1001     1002    35578 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sentence_hypothesis_or_recognition.py
+-rw-r--r--   0     1001     1002    31913 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py
+-rw-r--r--   0     1001     1002    34035 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sentence_recognition.py
+-rw-r--r--   0     1001     1002    30203 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/session_content.py
+-rw-r--r--   0     1001     1002    31715 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/session_error_response.py
+-rw-r--r--   0     1001     1002    37731 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/session_init_recognition.py
+-rw-r--r--   0     1001     1002    39973 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/session_init_transcription.py
+-rw-r--r--   0     1001     1002    33135 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/session_init_transcription_diarization.py
+-rw-r--r--   0     1001     1002    30937 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/session_success_response.py
+-rw-r--r--   0     1001     1002    35546 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/settings_async_transcription.py
+-rw-r--r--   0     1001     1002    32467 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/settings_recognition.py
+-rw-r--r--   0     1001     1002    32440 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/settings_sync_transcription.py
+-rw-r--r--   0     1001     1002    34452 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/silence.py
+-rw-r--r--   0     1001     1002    31098 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/slot_entity.py
+-rw-r--r--   0     1001     1002    31045 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/slot_keyword.py
+-rw-r--r--   0     1001     1002    31132 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sos_ref.py
+-rw-r--r--   0     1001     1002    33791 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speaker_result.py
+-rw-r--r--   0     1001     1002    44599 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_base_result.py
+-rw-r--r--   0     1001     1002    32274 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_channel.py
+-rw-r--r--   0     1001     1002    45972 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_channel_result.py
+-rw-r--r--   0     1001     1002    34258 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
+-rw-r--r--   0     1001     1002    71030 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config.py
+-rw-r--r--   0     1001     1002    34716 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_identifying.py
+-rw-r--r--   0     1001     1002    68305 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_modifiable.py
+-rw-r--r--   0     1001     1002    67025 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_modifiable_base.py
+-rw-r--r--   0     1001     1002    31583 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
+-rw-r--r--   0     1001     1002    31126 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_name_optional.py
+-rw-r--r--   0     1001     1002    31280 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_name_required.py
+-rw-r--r--   0     1001     1002    50326 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_core_result.py
+-rw-r--r--   0     1001     1002    35253 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_core_result_all_of.py
+-rw-r--r--   0     1001     1002    31192 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_criteria_data.py
+-rw-r--r--   0     1001     1002    31657 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_emotion.py
+-rw-r--r--   0     1001     1002    30860 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_emotion_data.py
+-rw-r--r--   0     1001     1002    36981 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_emotion_item.py
+-rw-r--r--   0     1001     1002    30906 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword.py
+-rw-r--r--   0     1001     1002    31196 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_data.py
+-rw-r--r--   0     1001     1002    36230 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_item.py
+-rw-r--r--   0     1001     1002    36482 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
+-rw-r--r--   0     1001     1002    32744 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py
+-rw-r--r--   0     1001     1002    31876 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity.py
+-rw-r--r--   0     1001     1002    37280 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity_item.py
+-rw-r--r--   0     1001     1002    37568 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
+-rw-r--r--   0     1001     1002    33818 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py
+-rw-r--r--   0     1001     1002    32962 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase.py
+-rw-r--r--   0     1001     1002    31179 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_data.py
+-rw-r--r--   0     1001     1002    33077 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_for_ws.py
+-rw-r--r--   0     1001     1002    31166 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py
+-rw-r--r--   0     1001     1002    31005 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group.py
+-rw-r--r--   0     1001     1002    31278 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group_data.py
+-rw-r--r--   0     1001     1002    31038 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py
+-rw-r--r--   0     1001     1002    36393 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group_item.py
+-rw-r--r--   0     1001     1002    38302 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_item.py
+-rw-r--r--   0     1001     1002    39702 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
+-rw-r--r--   0     1001     1002    31076 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_slots.py
+-rw-r--r--   0     1001     1002    61306 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_result.py
+-rw-r--r--   0     1001     1002    46633 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_result_detail.py
+-rw-r--r--   0     1001     1002    31091 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_session_modifiable.py
+-rw-r--r--   0     1001     1002    38026 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_session_poll_response.py
+-rw-r--r--   0     1001     1002    36321 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_websocket_payload.py
+-rw-r--r--   0     1001     1002    31728 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/start_end_time_for_sub_criterion.py
+-rw-r--r--   0     1001     1002    30414 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stomp_ping.py
+-rw-r--r--   0     1001     1002    33034 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stomp_word_correction.py
+-rw-r--r--   0     1001     1002    37053 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stomp_ws_word.py
+-rw-r--r--   0     1001     1002    31191 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stomp_ws_word_all_of.py
+-rw-r--r--   0     1001     1002    35348 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stomp_ws_word_base.py
+-rw-r--r--   0     1001     1002    35620 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stream_resp.py
+-rw-r--r--   0     1001     1002    33181 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/stream_setup.py
+-rw-r--r--   0     1001     1002    29634 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/streaming_protocol.py
+-rw-r--r--   0     1001     1002    38813 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sub_criterion_config.py
+-rw-r--r--   0     1001     1002    41199 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sub_criterion_satisfied.py
+-rw-r--r--   0     1001     1002    32174 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_audio_input_source.py
+-rw-r--r--   0     1001     1002    31122 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_recognition_request.py
+-rw-r--r--   0     1001     1002    32687 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_recognition_response.py
+-rw-r--r--   0     1001     1002    30290 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_session_established.py
+-rw-r--r--   0     1001     1002    31006 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_transcription_request.py
+-rw-r--r--   0     1001     1002    32745 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_transcription_response.py
+-rw-r--r--   0     1001     1002    33184 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/sync_transcription_result.py
+-rw-r--r--   0     1001     1002    38900 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/talk_time.py
+-rw-r--r--   0     1001     1002    31431 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/topic_score.py
+-rw-r--r--   0     1001     1002    29530 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_bucket_type.py
+-rw-r--r--   0     1001     1002    39172 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_doc.py
+-rw-r--r--   0     1001     1002    31090 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_doc_defaults.py
+-rw-r--r--   0     1001     1002    36550 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_doc_statistics.py
+-rw-r--r--   0     1001     1002    34624 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_key.py
+-rw-r--r--   0     1001     1002    33874 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_modifiable.py
+-rw-r--r--   0     1001     1002    29622 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_status.py
+-rw-r--r--   0     1001     1002    29662 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_status_modifiable.py
+-rw-r--r--   0     1001     1002    29550 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/training_set_store_type.py
+-rw-r--r--   0     1001     1002    31792 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcribe_alt.py
+-rw-r--r--   0     1001     1002    31074 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_id.py
+-rw-r--r--   0     1001     1002    34092 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_modify_request.py
+-rw-r--r--   0     1001     1002    31769 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_modify_request_mute.py
+-rw-r--r--   0     1001     1002    30597 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_modify_request_pause.py
+-rw-r--r--   0     1001     1002    34626 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcript_position_range.py
+-rw-r--r--   0     1001     1002    34806 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcript_position_range_for_phrase.py
+-rw-r--r--   0     1001     1002    36042 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
+-rw-r--r--   0     1001     1002    36363 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transfer.py
+-rw-r--r--   0     1001     1002    36503 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/transfer_all_of.py
+-rw-r--r--   0     1001     1002    29546 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/vad_mode.py
+-rw-r--r--   0     1001     1002    32351 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/version.py
+-rw-r--r--   0     1001     1002    38003 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket.py
+-rw-r--r--   0     1001     1002    41057 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket_init.py
+-rw-r--r--   0     1001     1002    30564 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket_init_reco.py
+-rw-r--r--   0     1001     1002    36159 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket_modifiable.py
+-rw-r--r--   0     1001     1002    32627 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket_msg.py
+-rw-r--r--   0     1001     1002    29493 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket_protocol.py
+-rw-r--r--   0     1001     1002    30968 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/websocket_resp.py
+-rw-r--r--   0     1001     1002    30325 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_alternatives.py
+-rw-r--r--   0     1001     1002    31505 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_cloud_item.py
+-rw-r--r--   0     1001     1002    31346 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_correction.py
+-rw-r--r--   0     1001     1002    36356 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_item_timed.py
+-rw-r--r--   0     1001     1002    31431 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_item_timing.py
+-rw-r--r--   0     1001     1002    30686 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_tree_ids.py
+-rw-r--r--   0     1001     1002    36733 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/word_tree_item.py
+-rw-r--r--   0     1001     1002    33288 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_item.py
+-rw-r--r--   0     1001     1002    36591 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_section.py
+-rw-r--r--   0     1001     1002    33137 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_section_meta.py
+-rw-r--r--   0     1001     1002    32139 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_section_meta_mc.py
+-rw-r--r--   0     1001     1002    34118 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_section_single_column.py
+-rw-r--r--   0     1001     1002    30199 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_section_words.py
+-rw-r--r--   0     1001     1002    44224 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/words_websocket_item.py
+-rw-r--r--   0     1001     1002    33875 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_emotion_item.py
+-rw-r--r--   0     1001     1002    33124 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_keyword_item.py
+-rw-r--r--   0     1001     1002    34114 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_named_entity_item.py
+-rw-r--r--   0     1001     1002    32348 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_phrase_group_item.py
+-rw-r--r--   0     1001     1002    35127 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_phrase_item.py
+-rw-r--r--   0     1001     1002    35479 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_phrase_item_inside_group.py
+-rw-r--r--   0     1001     1002    31700 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_position_range.py
+-rw-r--r--   0     1001     1002    30884 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_position_range_nested.py
+-rw-r--r--   0     1001     1002    30872 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_position_range_no_spk.py
+-rw-r--r--   0     1001     1002    37497 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py
+-rw-r--r--   0     1001     1002    31349 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py
+-rw-r--r--   0     1001     1002    32682 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_speaker.py
+-rw-r--r--   0     1001     1002    34542 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_word.py
+-rw-r--r--   0     1001     1002    32108 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/models/ws_word_edit.py
+-rw-r--r--   0     1001     1002    39169 2023-06-30 03:38:37.000000 voicegain-speech-1.85.2/voicegain_speech/rest.py
+drwxr-xr-x   0     1001     1002        0 2023-06-30 03:38:40.205337 voicegain-speech-1.85.2/voicegain_speech.egg-info/
+-rw-r--r--   0     1001     1002     2923 2023-06-30 03:38:40.000000 voicegain-speech-1.85.2/voicegain_speech.egg-info/PKG-INFO
+-rw-r--r--   0     1001     1002    22939 2023-06-30 03:38:40.000000 voicegain-speech-1.85.2/voicegain_speech.egg-info/SOURCES.txt
+-rw-r--r--   0     1001     1002        1 2023-06-30 03:38:40.000000 voicegain-speech-1.85.2/voicegain_speech.egg-info/dependency_links.txt
+-rw-r--r--   0     1001     1002       48 2023-06-30 03:38:40.000000 voicegain-speech-1.85.2/voicegain_speech.egg-info/requires.txt
+-rw-r--r--   0     1001     1002       17 2023-06-30 03:38:40.000000 voicegain-speech-1.85.2/voicegain_speech.egg-info/top_level.txt
```

### Comparing `voicegain-speech-1.85.1/LICENSE` & `voicegain-speech-1.85.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/PKG-INFO` & `voicegain-speech-1.85.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.85.1
+Version: 1.85.2
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.85.1.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.85.2.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.85.1/README.md` & `voicegain-speech-1.85.2/README.md`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/setup.py` & `voicegain-speech-1.85.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="voicegain-speech",
-    version="1.85.1",
+    version="1.85.2",
     author="Huishen Zhan, Kuo Zhang, Jacek Jarmulak",
     author_email="huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai",
     description="Voicegain Speech-to-Text Python SDK",
-    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.85.1.tar.gz',
+    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.85.2.tar.gz',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     packages=setuptools.find_packages(),
     include_package_data=True,
 )
```

### Comparing `voicegain-speech-1.85.1/voicegain_speech/__init__.py` & `voicegain-speech-1.85.2/voicegain_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/__init__.py` & `voicegain-speech-1.85.2/voicegain_speech/api/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/aivr_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/aivr_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/aivr_callback_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/aivr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/asr_callback_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/asr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/audiocodes_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/audiocodes_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/data_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/data_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/greg_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/greg_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/lm_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/lm_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/recognize_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/recognize_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/sa_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/sa_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/security_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/security_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/training_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/training_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/transcribe_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/transcribe_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api/websocket_api.py` & `voicegain-speech-1.85.2/voicegain_speech/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/api_client.py` & `voicegain-speech-1.85.2/voicegain_speech/api_client.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/configuration.py` & `voicegain-speech-1.85.2/voicegain_speech/configuration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/exceptions.py` & `voicegain-speech-1.85.2/voicegain_speech/exceptions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/__init__.py` & `voicegain-speech-1.85.2/voicegain_speech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_control_messages.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_control_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_end.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_end.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_error.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_hypothesis.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_hypothesis.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_hypothesis_alternatives.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_hypothesis_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_recognition_alternatives.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_response_messages.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_response_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_start.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_start.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_start_stt_speech_contexts.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_start_stt_speech_contexts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_started.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ac_stop.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ac_stop.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/account_and_context_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/account_and_context_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/advanced_regex.py` & `voicegain-speech-1.85.2/voicegain_speech/models/advanced_regex.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aircall.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aircall.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aircall_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aircall_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_callback_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_callback_response_final.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_callback_response_final.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_conference_transfer.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_conference_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_disconnect.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_event.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_event_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_event_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_existing_session.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_existing_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic_media.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic_media.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic_transfer.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_logic_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_logic_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_new_session.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_new_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_phone_transfer.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_phone_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_completion.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_completion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_playing.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_playing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_properties_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_prompt_properties_html.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_prompt_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_question.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_recognition_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_recording.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_recording.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_response_properties_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_response_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_response_properties_html.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_response_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_session_user.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_session_user.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_session_user_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_session_user_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_session_user_fs.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_session_user_fs.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivr_transfer.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivr_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/aivrs_question_specifics.py` & `voicegain-speech-1.85.2/voicegain_speech/models/aivrs_question_specifics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/answer_map_entry.py` & `voicegain-speech-1.85.2/voicegain_speech/models/answer_map_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_event.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status_additional.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status_additional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status_after_input_started.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status_after_input_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_processing_status_for_callback.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_processing_status_for_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_recognition_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_common.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition_defaults.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition_grammars_etc.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition_grammars_etc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_recognition_timeouts.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_recognition_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_async.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_async_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_async_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_common.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_common_lm.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_common_lm.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_default_timeouts.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_default_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_defaults.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_sa.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_sa.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_speakers.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/asr_transcribe_queue_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/asr_transcribe_queue_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_audio_input_source.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_mode.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_mode_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_mode_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_mode_speech_analytics.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_mode_speech_analytics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_mode_transcription.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_mode_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_post_response_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_post_response_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_post_response_base_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_post_response_base_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_reco_post_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_reco_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_reco_post_response_sessions.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_reco_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_callback_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_request.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_recognition_result_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_recognition_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio_callback.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio_source.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_full_all_of_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_full_all_of_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail_control_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail_control_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_session_established.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_session_short_info.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_session_short_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_session_url.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_session_url.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transc_post_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transc_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transc_post_response_sessions.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transc_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transc_session_established.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transc_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_callback_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_request.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/async_transcription_response_shared.py` & `voicegain-speech-1.85.2/voicegain_speech/models/async_transcription_response_shared.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_channel.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_channel_selector.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_channel_selector.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_channel_selector_offline_async.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_channel_selector_offline_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_channels.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_channels.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_for_data_object.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_for_data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_format.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_format.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_async.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_async_source.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_async_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_async_with_callback.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_async_with_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_callback.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_callback_callback.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_callback_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_data_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_data_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_data_all_of_source.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_data_all_of_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_sync.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_sync.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_input_sync_source.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_input_sync_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_resource_uri.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_zone_class.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_zone_class.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/audio_zone_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/audio_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/basic_success_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/basic_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/builtin.py` & `voicegain-speech-1.85.2/voicegain_speech/models/builtin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/builtin_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/builtin_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/call_attributes.py` & `voicegain-speech-1.85.2/voicegain_speech/models/call_attributes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/call_review_answer_alone.py` & `voicegain-speech-1.85.2/voicegain_speech/models/call_review_answer_alone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/call_review_answer_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/call_review_answer_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/call_review_config_question_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/call_review_config_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/call_review_config_question_base_with_answer.py` & `voicegain-speech-1.85.2/voicegain_speech/models/call_review_config_question_base_with_answer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/call_review_config_question_base_with_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/call_review_config_question_base_with_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/callback_req.py` & `voicegain-speech-1.85.2/voicegain_speech/models/callback_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/callback_req_reco.py` & `voicegain-speech-1.85.2/voicegain_speech/models/callback_req_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/callback_resp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/callback_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/caption.py` & `voicegain-speech-1.85.2/voicegain_speech/models/caption.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/compliance_settings.py` & `voicegain-speech-1.85.2/voicegain_speech/models/compliance_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/config_value_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/config_value_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/content_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/content_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/continuous_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/continuous_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/core_aivr_session.py` & `voicegain-speech-1.85.2/voicegain_speech/models/core_aivr_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/core_aivr_session_telco_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/core_aivr_session_telco_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/cr_question_id_for_cr_config.py` & `voicegain-speech-1.85.2/voicegain_speech/models/cr_question_id_for_cr_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/creating_entity.py` & `voicegain-speech-1.85.2/voicegain_speech/models/creating_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/criterion_config.py` & `voicegain-speech-1.85.2/voicegain_speech/models/criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/criterion_satisfied.py` & `voicegain-speech-1.85.2/voicegain_speech/models/criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_obj_ref.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_obj_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_object.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_object_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_object_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_object_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_object_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_object_ids.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_object_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_object_no_sos_ref.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_object_no_sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/data_object_with_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/data_object_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/debug_info.py` & `voicegain-speech-1.85.2/voicegain_speech/models/debug_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/debug_settings.py` & `voicegain-speech-1.85.2/voicegain_speech/models/debug_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/demo.py` & `voicegain-speech-1.85.2/voicegain_speech/models/demo.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/demo_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/demo_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/diarization_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/diarization_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/diarization_zone.py` & `voicegain-speech-1.85.2/voicegain_speech/models/diarization_zone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/diarization_zone_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/diarization_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/disconnect.py` & `voicegain-speech-1.85.2/voicegain_speech/models/disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/disconnect_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/disconnect_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/error.py` & `voicegain-speech-1.85.2/voicegain_speech/models/error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/error_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/error_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/error_info.py` & `voicegain-speech-1.85.2/voicegain_speech/models/error_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/estimated_queue_wait.py` & `voicegain-speech-1.85.2/voicegain_speech/models/estimated_queue_wait.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/experiment_platform.py` & `voicegain-speech-1.85.2/voicegain_speech/models/experiment_platform.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/file_location.py` & `voicegain-speech-1.85.2/voicegain_speech/models/file_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/formatter.py` & `voicegain-speech-1.85.2/voicegain_speech/models/formatter.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/grammar.py` & `voicegain-speech-1.85.2/voicegain_speech/models/grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_base_with_audio.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_base_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input_audio_hash.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input_audio_hash.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input_audio_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_input_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_base_inclusive.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_core.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_inclusive.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_inclusive_core.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_inclusive_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_inner.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_set_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_set_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_audio_thin.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_audio_thin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_base_inclusive.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_base_platform_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_base_platform_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_inclusive.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_platform_external_asr.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_platform_external_asr.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_platform_upload.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_platform_upload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_platform_voicegain.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_platform_voicegain.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_experiment_status_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_experiment_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_base_light.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_base_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_inner.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_grammar_light.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_grammar_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_interpretation.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_interpretation.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_question.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_question_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_question_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_question_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_question_inner.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_question_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recog_base_with_exp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recog_base_with_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recognition_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recognition_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_recognition_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_recognition_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_review_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_review_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_source_of_truth.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_source_of_truth.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_truth_update.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_truth_update.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/greg_truth_updates.py` & `voicegain-speech-1.85.2/voicegain_speech/models/greg_truth_updates.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/grxml.py` & `voicegain-speech-1.85.2/voicegain_speech/models/grxml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/grxml_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/grxml_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/gui_input.py` & `voicegain-speech-1.85.2/voicegain_speech/models/gui_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/hangup.py` & `voicegain-speech-1.85.2/voicegain_speech/models/hangup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/html_checkbox.py` & `voicegain-speech-1.85.2/voicegain_speech/models/html_checkbox.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/html_choice_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/html_choice_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/html_radio_buttons.py` & `voicegain-speech-1.85.2/voicegain_speech/models/html_radio_buttons.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/html_text_entry.py` & `voicegain-speech-1.85.2/voicegain_speech/models/html_text_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/if_exists.py` & `voicegain-speech-1.85.2/voicegain_speech/models/if_exists.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/incident.py` & `voicegain-speech-1.85.2/voicegain_speech/models/incident.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/inline_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/inline_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/inline_object.py` & `voicegain-speech-1.85.2/voicegain_speech/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/inline_object1.py` & `voicegain-speech-1.85.2/voicegain_speech/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/input.py` & `voicegain-speech-1.85.2/voicegain_speech/models/input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/input_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/input_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/integration.py` & `voicegain-speech-1.85.2/voicegain_speech/models/integration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/jjsgf.py` & `voicegain-speech-1.85.2/voicegain_speech/models/jjsgf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/jjsgf_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/jjsgf_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/keyword_spot_example.py` & `voicegain-speech-1.85.2/voicegain_speech/models/keyword_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/keyword_spot_group.py` & `voicegain-speech-1.85.2/voicegain_speech/models/keyword_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/keyword_spot_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/keyword_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/lang_model_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/lang_model_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/language.py` & `voicegain-speech-1.85.2/voicegain_speech/models/language.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/language_model_doc.py` & `voicegain-speech-1.85.2/voicegain_speech/models/language_model_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/language_model_doc_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/language_model_doc_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/language_model_src_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/language_model_src_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/lm_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/lm_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/min_max_speakers.py` & `voicegain-speech-1.85.2/voicegain_speech/models/min_max_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/min_max_speakers_diarization.py` & `voicegain-speech-1.85.2/voicegain_speech/models/min_max_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/mood_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/mood_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/mrc_pv1_asr_settings.py` & `voicegain-speech-1.85.2/voicegain_speech/models/mrc_pv1_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/mrc_pv2_asr_settings.py` & `voicegain-speech-1.85.2/voicegain_speech/models/mrc_pv2_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/mrcp_version.py` & `voicegain-speech-1.85.2/voicegain_speech/models/mrcp_version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/multipart_form_data_field.py` & `voicegain-speech-1.85.2/voicegain_speech/models/multipart_form_data_field.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/name_value_pair.py` & `voicegain-speech-1.85.2/voicegain_speech/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/named_entity_concept.py` & `voicegain-speech-1.85.2/voicegain_speech/models/named_entity_concept.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/named_entity_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/named_entity_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session.py` & `voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session_response_poll.py` & `voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session_response_poll.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/new_speech_analytics_session_response_websocket.py` & `voicegain-speech-1.85.2/voicegain_speech/models/new_speech_analytics_session_response_websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/non_session_error_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/non_session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/non_session_error_response400.py` & `voicegain-speech-1.85.2/voicegain_speech/models/non_session_error_response400.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/non_session_error_response401.py` & `voicegain-speech-1.85.2/voicegain_speech/models/non_session_error_response401.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/output.py` & `voicegain-speech-1.85.2/voicegain_speech/models/output.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/output_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/output_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/overtalk.py` & `voicegain-speech-1.85.2/voicegain_speech/models/overtalk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phone_audio_input.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phone_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phone_audio_input_prompt.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phone_audio_input_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_example.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_group.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item_location.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item_location_dialogue.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item_location_dialogue.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/phrase_spot_item_slots.py` & `voicegain-speech-1.85.2/voicegain_speech/models/phrase_spot_item_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/pii_redaction_conf.py` & `voicegain-speech-1.85.2/voicegain_speech/models/pii_redaction_conf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/poll_req.py` & `voicegain-speech-1.85.2/voicegain_speech/models/poll_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/poll_resp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/poll_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/portal_output_init.py` & `voicegain-speech-1.85.2/voicegain_speech/models/portal_output_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/pre_fetch.py` & `voicegain-speech-1.85.2/voicegain_speech/models/pre_fetch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/progress.py` & `voicegain-speech-1.85.2/voicegain_speech/models/progress.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/progress_callback.py` & `voicegain-speech-1.85.2/voicegain_speech/models/progress_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/progress_phase.py` & `voicegain-speech-1.85.2/voicegain_speech/models/progress_phase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/quartiles_energy.py` & `voicegain-speech-1.85.2/voicegain_speech/models/quartiles_energy.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/quartiles_pitch.py` & `voicegain-speech-1.85.2/voicegain_speech/models/quartiles_pitch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/reco_alt.py` & `voicegain-speech-1.85.2/voicegain_speech/models/reco_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/recog_nlsml.py` & `voicegain-speech-1.85.2/voicegain_speech/models/recog_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/recog_nlsml_no_exp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/recog_nlsml_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/recog_obj.py` & `voicegain-speech-1.85.2/voicegain_speech/models/recog_obj.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/recog_obj_no_exp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/recog_obj_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/recognition_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/requested_content.py` & `voicegain-speech-1.85.2/voicegain_speech/models/requested_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/resource_uri.py` & `voicegain-speech-1.85.2/voicegain_speech/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/results_websocket_mode.py` & `voicegain-speech-1.85.2/voicegain_speech/models/results_websocket_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/s3.py` & `voicegain-speech-1.85.2/voicegain_speech/models/s3.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/s3_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/s3_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/s3_audio_input.py` & `voicegain-speech-1.85.2/voicegain_speech/models/s3_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/s3_metadata_mapping.py` & `voicegain-speech-1.85.2/voicegain_speech/models/s3_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/s3_tag_mapping.py` & `voicegain-speech-1.85.2/voicegain_speech/models/s3_tag_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sa_conf_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sa_conf_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sample_rate.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sample_rate.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sentence_hypothesis_or_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sentence_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sentence_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/session_content.py` & `voicegain-speech-1.85.2/voicegain_speech/models/session_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/session_error_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/session_init_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/session_init_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/session_init_transcription.py` & `voicegain-speech-1.85.2/voicegain_speech/models/session_init_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/session_init_transcription_diarization.py` & `voicegain-speech-1.85.2/voicegain_speech/models/session_init_transcription_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/session_success_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/session_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/settings_async_transcription.py` & `voicegain-speech-1.85.2/voicegain_speech/models/settings_async_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/settings_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/settings_sync_transcription.py` & `voicegain-speech-1.85.2/voicegain_speech/models/settings_sync_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/silence.py` & `voicegain-speech-1.85.2/voicegain_speech/models/silence.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/slot_entity.py` & `voicegain-speech-1.85.2/voicegain_speech/models/slot_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/slot_keyword.py` & `voicegain-speech-1.85.2/voicegain_speech/models/slot_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sos_ref.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speaker_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speaker_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_base_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_base_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_channel.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_channel_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_channel_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_channel_with_transcribe.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_channel_with_transcribe.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_identifying.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_identifying.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_modifiable_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_modifiable_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_name_optional.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_name_optional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_config_name_required.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_config_name_required.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_core_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_core_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_core_result_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_core_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_criteria_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_criteria_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_emotion.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_emotion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_emotion_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_emotion_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_emotion_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_for_ws.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group_data.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_group_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_phrase_slots.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_phrase_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_result_detail.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_result_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_session_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_session_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_session_poll_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_session_poll_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/speech_analytics_websocket_payload.py` & `voicegain-speech-1.85.2/voicegain_speech/models/speech_analytics_websocket_payload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/start_end_time_for_sub_criterion.py` & `voicegain-speech-1.85.2/voicegain_speech/models/start_end_time_for_sub_criterion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stomp_ping.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stomp_ping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stomp_word_correction.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stomp_word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stomp_ws_word.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stomp_ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stomp_ws_word_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stomp_ws_word_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stomp_ws_word_base.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stomp_ws_word_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stream_resp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stream_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/stream_setup.py` & `voicegain-speech-1.85.2/voicegain_speech/models/stream_setup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/streaming_protocol.py` & `voicegain-speech-1.85.2/voicegain_speech/models/streaming_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sub_criterion_config.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sub_criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sub_criterion_satisfied.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sub_criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_audio_input_source.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_recognition_request.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_recognition_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_session_established.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_transcription_request.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_transcription_response.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/sync_transcription_result.py` & `voicegain-speech-1.85.2/voicegain_speech/models/sync_transcription_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/talk_time.py` & `voicegain-speech-1.85.2/voicegain_speech/models/talk_time.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/topic_score.py` & `voicegain-speech-1.85.2/voicegain_speech/models/topic_score.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_bucket_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_bucket_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_doc.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_doc_defaults.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_doc_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_doc_statistics.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_doc_statistics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_key.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_key.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_status.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_status_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/training_set_store_type.py` & `voicegain-speech-1.85.2/voicegain_speech/models/training_set_store_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcribe_alt.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcribe_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_id.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_modify_request.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_modify_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_modify_request_mute.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_modify_request_mute.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcribe_session_modify_request_pause.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcribe_session_modify_request_pause.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcript_position_range.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcript_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcript_position_range_for_phrase.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcript_position_range_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transfer.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/transfer_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/transfer_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/vad_mode.py` & `voicegain-speech-1.85.2/voicegain_speech/models/vad_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/version.py` & `voicegain-speech-1.85.2/voicegain_speech/models/version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket_init.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket_init_reco.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket_init_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket_modifiable.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket_msg.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket_msg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket_protocol.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/websocket_resp.py` & `voicegain-speech-1.85.2/voicegain_speech/models/websocket_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_alternatives.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_cloud_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_cloud_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_correction.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_item_timed.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_item_timed.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_item_timing.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_item_timing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_tree_ids.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_tree_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/word_tree_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/word_tree_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_section.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_section.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_section_meta.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_section_meta.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_section_meta_mc.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_section_meta_mc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_section_single_column.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_section_single_column.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_section_words.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_section_words.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/words_websocket_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/words_websocket_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_emotion_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_keyword_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_named_entity_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_phrase_group_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_phrase_item.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_phrase_item_inside_group.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_phrase_item_inside_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_position_range.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_position_range_nested.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_position_range_nested.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sa_position_range_no_spk.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sa_position_range_no_spk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_speaker.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_speaker.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_word.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/models/ws_word_edit.py` & `voicegain-speech-1.85.2/voicegain_speech/models/ws_word_edit.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech/rest.py` & `voicegain-speech-1.85.2/voicegain_speech/rest.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.85.1/voicegain_speech.egg-info/PKG-INFO` & `voicegain-speech-1.85.2/voicegain_speech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.85.1
+Version: 1.85.2
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.85.1.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.85.2.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.85.1/voicegain_speech.egg-info/SOURCES.txt` & `voicegain-speech-1.85.2/voicegain_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

