# Comparing `tmp/getajob-0.6.1.tar.gz` & `tmp/getajob-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.6.1.tar", max compression
+gzip compressed data, was "getajob-0.6.2.tar", max compression
```

## Comparing `getajob-0.6.1.tar` & `getajob-0.6.2.tar`

### file list

```diff
@@ -1,184 +1,184 @@
--rw-r--r--   0        0        0    11357 2023-08-03 15:28:45.600914 getajob-0.6.1/LICENSE
--rw-r--r--   0        0        0       69 2023-08-03 15:28:45.600914 getajob-0.6.1/README.md
--rw-r--r--   0        0        0       22 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/__init__.py
--rw-r--r--   0        0        0     2980 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/abstractions/models.py
--rw-r--r--   0        0        0    16306 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/abstractions/repository.py
--rw-r--r--   0        0        0      385 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/abstractions/vendor_client_factory.py
--rw-r--r--   0        0        0     2161 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      177 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      607 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      844 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/applicant_tracking/__init__.py
--rw-r--r--   0        0        0     1044 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/applicant_tracking/models.py
--rw-r--r--   0        0        0     2502 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/applicant_tracking/repository.py
--rw-r--r--   0        0        0     4438 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/async_service.py
--rw-r--r--   0        0        0      277 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/enumerations.py
--rw-r--r--   0        0        0     1851 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     3804 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     1781 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/search.py
--rw-r--r--   0        0        0     2629 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/__init__.py
--rw-r--r--   0        0        0     2617 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/async_service.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/message/__init__.py
--rw-r--r--   0        0        0      616 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/message/models.py
--rw-r--r--   0        0        0      892 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/message/repository.py
--rw-r--r--   0        0        0      272 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/models.py
--rw-r--r--   0        0        0     1899 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/repository.py
--rw-r--r--   0        0        0     1650 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/chat/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/companies/applicant_tracking_settings/__init__.py
--rw-r--r--   0        0        0      368 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/companies/applicant_tracking_settings/models.py
--rw-r--r--   0        0        0      820 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/companies/applicant_tracking_settings/repository.py
--rw-r--r--   0        0        0     2375 2023-08-03 15:28:45.600914 getajob-0.6.1/getajob/contexts/companies/async_service.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/audit/__init__.py
--rw-r--r--   0        0        0     2100 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/audit/async_service.py
--rw-r--r--   0        0        0      482 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/audit/models.py
--rw-r--r--   0        0        0     1104 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/audit/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/details/__init__.py
--rw-r--r--   0        0        0      743 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/details/models.py
--rw-r--r--   0        0        0     1448 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/details/repository.py
--rw-r--r--   0        0        0     1870 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/enumerations.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/invitations/__init__.py
--rw-r--r--   0        0        0      145 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/invitations/models.py
--rw-r--r--   0        0        0      786 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/invitations/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/jobs/__init__.py
--rw-r--r--   0        0        0     3865 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/jobs/async_service.py
--rw-r--r--   0        0        0     3174 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/jobs/models.py
--rw-r--r--   0        0        0     1421 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/jobs/repository.py
--rw-r--r--   0        0        0      533 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/jobs/unit_of_work.py
--rw-r--r--   0        0        0      102 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/recruiters/__init__.py
--rw-r--r--   0        0        0      117 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/recruiters/models.py
--rw-r--r--   0        0        0      744 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/recruiters/repository.py
--rw-r--r--   0        0        0     1357 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0      210 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/scheduled_events/enumerations.py
--rw-r--r--   0        0        0      995 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1865 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/search/__init__.py
--rw-r--r--   0        0        0     1732 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/search/models.py
--rw-r--r--   0        0        0     5410 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/async_service.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      854 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/details/__init__.py
--rw-r--r--   0        0        0     2974 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/details/models.py
--rw-r--r--   0        0        0     1416 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/details/repository.py
--rw-r--r--   0        0        0     1213 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/enumerations.py
--rw-r--r--   0        0        0       89 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/models.py
--rw-r--r--   0        0        0     1362 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/__init__.py
--rw-r--r--   0        0        0     7626 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/extractor.py
--rw-r--r--   0        0        0     1966 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/models.py
--rw-r--r--   0        0        0     1629 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/repository.py
--rw-r--r--   0        0        0     1676 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/unit_of_work.py
--rw-r--r--   0        0        0      402 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0     1693 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0     2649 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json
--rw-r--r--   0        0        0     3412 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json
--rw-r--r--   0        0        0     1591 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json
--rw-r--r--   0        0        0     4311 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json
--rw-r--r--   0        0        0     2018 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json
--rw-r--r--   0        0        0     2479 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json
--rw-r--r--   0        0        0     2333 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json
--rw-r--r--   0        0        0     1844 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json
--rw-r--r--   0        0        0     4264 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json
--rw-r--r--   0        0        0     1806 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json
--rw-r--r--   0        0        0     2523 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json
--rw-r--r--   0        0        0     2028 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json
--rw-r--r--   0        0        0   107453 2023-08-03 15:28:45.604914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf
--rw-r--r--   0        0        0   173006 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf
--rw-r--r--   0        0        0   107503 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf
--rw-r--r--   0        0        0   111154 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf
--rw-r--r--   0        0        0   107645 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf
--rw-r--r--   0        0        0    30834 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf
--rw-r--r--   0        0        0    30608 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf
--rw-r--r--   0        0        0    31147 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf
--rw-r--r--   0        0        0   107907 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf
--rw-r--r--   0        0        0   106257 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf
--rw-r--r--   0        0        0   121496 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf
--rw-r--r--   0        0        0   106308 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf
--rw-r--r--   0        0        0     2628 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/resumes/unt_of_work.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      481 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0     2607 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/static/__init__.py
--rw-r--r--   0        0        0     1518 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/static/enumerations.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/__init__.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/__init__.py
--rw-r--r--   0        0        0     2286 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/application.py
--rw-r--r--   0        0        0     1750 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/chat.py
--rw-r--r--   0        0        0     1027 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/company.py
--rw-r--r--   0        0        0      408 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/job.py
--rw-r--r--   0        0        0     1843 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/recruiter.py
--rw-r--r--   0        0        0      645 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/recruiter_invitation.py
--rw-r--r--   0        0        0     1720 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/scheduled_events.py
--rw-r--r--   0        0        0     2579 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/test_support/fixtures/users.py
--rw-r--r--   0        0        0     1453 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/algolia/__init__.py
--rw-r--r--   0        0        0      468 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/algolia/client_factory.py
--rw-r--r--   0        0        0     2359 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/algolia/mock.py
--rw-r--r--   0        0        0      761 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     2352 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0     2139 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/client.py
--rw-r--r--   0        0        0      340 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/client_factory.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     2427 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0     1735 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/companies/unit_of_work.py
--rw-r--r--   0        0        0     2553 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/mock.py
--rw-r--r--   0        0        0      413 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2057 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1588 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2385 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     2318 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1353 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     2702 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firebase_storage/__init__.py
--rw-r--r--   0        0        0      846 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firebase_storage/client_factory.py
--rw-r--r--   0        0        0      953 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firebase_storage/mock.py
--rw-r--r--   0        0        0     1727 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firebase_storage/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firestore/__init__.py
--rw-r--r--   0        0        0      749 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firestore/client_factory.py
--rw-r--r--   0        0        0     1102 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firestore/helpers.py
--rw-r--r--   0        0        0      507 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firestore/mock.py
--rw-r--r--   0        0        0     1975 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firestore/models.py
--rw-r--r--   0        0        0     9200 2023-08-03 15:28:45.608914 getajob-0.6.1/getajob/vendor/firestore/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      725 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0     1369 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/client_factory.py
--rw-r--r--   0        0        0      320 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0      716 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     2178 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0     1517 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/mailgun/__init__.py
--rw-r--r--   0        0        0      989 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/mailgun/client_factory.py
--rw-r--r--   0        0        0      282 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/mailgun/mock.py
--rw-r--r--   0        0        0     1231 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/mailgun/repository.py
--rw-r--r--   0        0        0      104 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/mailgun/templates/chat_message.html
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/openai/__init__.py
--rw-r--r--   0        0        0      447 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/openai/client_factory.py
--rw-r--r--   0        0        0      521 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/openai/mock.py
--rw-r--r--   0        0        0     1185 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/openai/repository.py
--rw-r--r--   0        0        0      572 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/openai/settings.py
--rw-r--r--   0        0        0        0 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/redis/__init__.py
--rw-r--r--   0        0        0      508 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/redis/client_factory.py
--rw-r--r--   0        0        0      343 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/redis/mock.py
--rw-r--r--   0        0        0     2463 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/redis/repository.py
--rw-r--r--   0        0        0      251 2023-08-03 15:28:45.612914 getajob-0.6.1/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1809 2023-08-03 15:28:45.612914 getajob-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 getajob-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-03 17:06:10.608856 getajob-0.6.2/LICENSE
+-rw-r--r--   0        0        0       69 2023-08-03 17:06:10.608856 getajob-0.6.2/README.md
+-rw-r--r--   0        0        0       22 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/__init__.py
+-rw-r--r--   0        0        0     2980 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/abstractions/models.py
+-rw-r--r--   0        0        0    16306 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0      385 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/abstractions/vendor_client_factory.py
+-rw-r--r--   0        0        0     2161 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      177 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      607 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-08-03 17:06:10.608856 getajob-0.6.2/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      844 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/applicant_tracking/__init__.py
+-rw-r--r--   0        0        0     1044 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/applicant_tracking/models.py
+-rw-r--r--   0        0        0     2502 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/applicant_tracking/repository.py
+-rw-r--r--   0        0        0     4438 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/async_service.py
+-rw-r--r--   0        0        0      277 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/enumerations.py
+-rw-r--r--   0        0        0     1851 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     3804 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     1781 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/search.py
+-rw-r--r--   0        0        0     2629 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/__init__.py
+-rw-r--r--   0        0        0     2617 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/message/__init__.py
+-rw-r--r--   0        0        0      616 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/message/models.py
+-rw-r--r--   0        0        0      892 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/message/repository.py
+-rw-r--r--   0        0        0      272 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/models.py
+-rw-r--r--   0        0        0     1899 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/repository.py
+-rw-r--r--   0        0        0     1650 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/chat/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/applicant_tracking_settings/__init__.py
+-rw-r--r--   0        0        0      368 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/applicant_tracking_settings/models.py
+-rw-r--r--   0        0        0      820 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/applicant_tracking_settings/repository.py
+-rw-r--r--   0        0        0     2375 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/audit/__init__.py
+-rw-r--r--   0        0        0     2100 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/audit/async_service.py
+-rw-r--r--   0        0        0      482 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/audit/models.py
+-rw-r--r--   0        0        0     1104 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/audit/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/details/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/details/models.py
+-rw-r--r--   0        0        0     1448 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/details/repository.py
+-rw-r--r--   0        0        0     1870 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/enumerations.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      786 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/jobs/__init__.py
+-rw-r--r--   0        0        0     3865 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/jobs/async_service.py
+-rw-r--r--   0        0        0     3174 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/jobs/models.py
+-rw-r--r--   0        0        0     1421 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/jobs/repository.py
+-rw-r--r--   0        0        0      533 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      102 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0      744 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0     1357 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0      210 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/scheduled_events/enumerations.py
+-rw-r--r--   0        0        0      995 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1865 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/search/__init__.py
+-rw-r--r--   0        0        0     1732 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/search/models.py
+-rw-r--r--   0        0        0     5410 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      854 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/details/__init__.py
+-rw-r--r--   0        0        0     2974 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/details/models.py
+-rw-r--r--   0        0        0     1416 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/details/repository.py
+-rw-r--r--   0        0        0     1213 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/enumerations.py
+-rw-r--r--   0        0        0       89 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0     1362 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/__init__.py
+-rw-r--r--   0        0        0     7626 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/extractor.py
+-rw-r--r--   0        0        0     1966 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/models.py
+-rw-r--r--   0        0        0     1630 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/repository.py
+-rw-r--r--   0        0        0     1676 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/unit_of_work.py
+-rw-r--r--   0        0        0      402 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0     1693 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0     2649 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json
+-rw-r--r--   0        0        0     3412 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json
+-rw-r--r--   0        0        0     1591 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json
+-rw-r--r--   0        0        0     4311 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json
+-rw-r--r--   0        0        0     2018 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json
+-rw-r--r--   0        0        0     2479 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json
+-rw-r--r--   0        0        0     2333 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json
+-rw-r--r--   0        0        0     1844 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json
+-rw-r--r--   0        0        0     4264 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json
+-rw-r--r--   0        0        0     1806 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json
+-rw-r--r--   0        0        0     2523 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json
+-rw-r--r--   0        0        0     2028 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json
+-rw-r--r--   0        0        0   107453 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf
+-rw-r--r--   0        0        0   173006 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf
+-rw-r--r--   0        0        0   107503 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf
+-rw-r--r--   0        0        0   111154 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf
+-rw-r--r--   0        0        0   107645 2023-08-03 17:06:10.612856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf
+-rw-r--r--   0        0        0    30834 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf
+-rw-r--r--   0        0        0    30608 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf
+-rw-r--r--   0        0        0    31147 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf
+-rw-r--r--   0        0        0   107907 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf
+-rw-r--r--   0        0        0   106257 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf
+-rw-r--r--   0        0        0   121496 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf
+-rw-r--r--   0        0        0   106308 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf
+-rw-r--r--   0        0        0     2628 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/resumes/unt_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0     2607 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/static/__init__.py
+-rw-r--r--   0        0        0     1518 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/static/enumerations.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/__init__.py
+-rw-r--r--   0        0        0     2286 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/application.py
+-rw-r--r--   0        0        0     1750 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/chat.py
+-rw-r--r--   0        0        0     1027 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/company.py
+-rw-r--r--   0        0        0      408 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/job.py
+-rw-r--r--   0        0        0     1843 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/recruiter.py
+-rw-r--r--   0        0        0      645 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/recruiter_invitation.py
+-rw-r--r--   0        0        0     1720 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/scheduled_events.py
+-rw-r--r--   0        0        0     2579 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/test_support/fixtures/users.py
+-rw-r--r--   0        0        0     1453 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/algolia/__init__.py
+-rw-r--r--   0        0        0      468 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/algolia/client_factory.py
+-rw-r--r--   0        0        0     2359 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/algolia/mock.py
+-rw-r--r--   0        0        0      758 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     2506 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0     2139 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/client.py
+-rw-r--r--   0        0        0      340 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/client_factory.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     2427 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0     1735 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/companies/unit_of_work.py
+-rw-r--r--   0        0        0     2553 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/mock.py
+-rw-r--r--   0        0        0      413 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2057 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1588 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2385 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     2318 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1353 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     2702 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firebase_storage/__init__.py
+-rw-r--r--   0        0        0      846 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firebase_storage/client_factory.py
+-rw-r--r--   0        0        0      953 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firebase_storage/mock.py
+-rw-r--r--   0        0        0     1727 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firebase_storage/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firestore/__init__.py
+-rw-r--r--   0        0        0      749 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firestore/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firestore/helpers.py
+-rw-r--r--   0        0        0      507 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firestore/mock.py
+-rw-r--r--   0        0        0     1975 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firestore/models.py
+-rw-r--r--   0        0        0     9200 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/firestore/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      725 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0     1369 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/client_factory.py
+-rw-r--r--   0        0        0      320 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0      716 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     2178 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0     1517 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/mailgun/__init__.py
+-rw-r--r--   0        0        0      989 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/mailgun/client_factory.py
+-rw-r--r--   0        0        0      282 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/mailgun/mock.py
+-rw-r--r--   0        0        0     1231 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/mailgun/repository.py
+-rw-r--r--   0        0        0      104 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/mailgun/templates/chat_message.html
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/openai/__init__.py
+-rw-r--r--   0        0        0      447 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/openai/client_factory.py
+-rw-r--r--   0        0        0      521 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/openai/mock.py
+-rw-r--r--   0        0        0     1185 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/openai/repository.py
+-rw-r--r--   0        0        0      572 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/openai/settings.py
+-rw-r--r--   0        0        0        0 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/redis/__init__.py
+-rw-r--r--   0        0        0      508 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/redis/client_factory.py
+-rw-r--r--   0        0        0      343 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/redis/mock.py
+-rw-r--r--   0        0        0     2463 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/redis/repository.py
+-rw-r--r--   0        0        0      251 2023-08-03 17:06:10.616856 getajob-0.6.2/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1809 2023-08-03 17:06:10.620857 getajob-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 getajob-0.6.2/PKG-INFO
```

### Comparing `getajob-0.6.1/LICENSE` & `getajob-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/abstractions/models.py` & `getajob-0.6.2/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/abstractions/repository.py` & `getajob-0.6.2/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/config/settings.py` & `getajob-0.6.2/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/admin/search/repository.py` & `getajob-0.6.2/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/admin/users/models.py` & `getajob-0.6.2/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/admin/users/repository.py` & `getajob-0.6.2/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/applicant_tracking/models.py` & `getajob-0.6.2/getajob/contexts/applications/applicant_tracking/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/applicant_tracking/repository.py` & `getajob-0.6.2/getajob/contexts/applications/applicant_tracking/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/async_service.py` & `getajob-0.6.2/getajob/contexts/applications/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/models.py` & `getajob-0.6.2/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/repository.py` & `getajob-0.6.2/getajob/contexts/applications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/search.py` & `getajob-0.6.2/getajob/contexts/applications/search.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/applications/unit_of_work.py` & `getajob-0.6.2/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/chat/async_service.py` & `getajob-0.6.2/getajob/contexts/chat/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/chat/message/models.py` & `getajob-0.6.2/getajob/contexts/chat/message/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/chat/message/repository.py` & `getajob-0.6.2/getajob/contexts/chat/message/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/chat/repository.py` & `getajob-0.6.2/getajob/contexts/chat/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/chat/unit_of_work.py` & `getajob-0.6.2/getajob/contexts/chat/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/applicant_tracking_settings/repository.py` & `getajob-0.6.2/getajob/contexts/companies/applicant_tracking_settings/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/async_service.py` & `getajob-0.6.2/getajob/contexts/companies/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/audit/async_service.py` & `getajob-0.6.2/getajob/contexts/companies/audit/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/audit/repository.py` & `getajob-0.6.2/getajob/contexts/companies/audit/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/details/models.py` & `getajob-0.6.2/getajob/contexts/companies/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/details/repository.py` & `getajob-0.6.2/getajob/contexts/companies/details/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/enumerations.py` & `getajob-0.6.2/getajob/contexts/companies/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/invitations/repository.py` & `getajob-0.6.2/getajob/contexts/companies/invitations/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/jobs/async_service.py` & `getajob-0.6.2/getajob/contexts/companies/jobs/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/jobs/models.py` & `getajob-0.6.2/getajob/contexts/companies/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/jobs/repository.py` & `getajob-0.6.2/getajob/contexts/companies/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/jobs/unit_of_work.py` & `getajob-0.6.2/getajob/contexts/companies/jobs/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/recruiters/repository.py` & `getajob-0.6.2/getajob/contexts/companies/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/companies/repository.py` & `getajob-0.6.2/getajob/contexts/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/scheduled_events/models.py` & `getajob-0.6.2/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/scheduled_events/repository.py` & `getajob-0.6.2/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/search/models.py` & `getajob-0.6.2/getajob/contexts/search/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/async_service.py` & `getajob-0.6.2/getajob/contexts/users/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.6.2/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/details/models.py` & `getajob-0.6.2/getajob/contexts/users/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/details/repository.py` & `getajob-0.6.2/getajob/contexts/users/details/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/enumerations.py` & `getajob-0.6.2/getajob/contexts/users/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/repository.py` & `getajob-0.6.2/getajob/contexts/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/extractor.py` & `getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/extractor.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/models.py` & `getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/repository.py` & `getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ):
         self.request_scope = request_scope
         super().__init__(
             RepositoryDependencies(
                 user_id=request_scope.initiating_user_id,
                 db=request_scope.db,
                 collection_name=Entity.USER_DETAILS.value,
-                entity_models=entity_models
+                entity_models=entity_models,
             ),
             required_parent_keys=[Entity.USERS.value, Entity.RESUMES.value],
         )
 
     async def create_resume_extraction(self, user_id: str, resume_id: str):
         return await ResumeExtractorUnitOfWork(
             resume_repo=ResumeRepository(request_scope=self.request_scope),
```

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/extracted_data/unit_of_work.py` & `getajob-0.6.2/getajob/contexts/users/resumes/extracted_data/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/repository.py` & `getajob-0.6.2/getajob/contexts/users/resumes/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf` & `getajob-0.6.2/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/contexts/users/resumes/unt_of_work.py` & `getajob-0.6.2/getajob/contexts/users/resumes/unt_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/exceptions.py` & `getajob-0.6.2/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/static/enumerations.py` & `getajob-0.6.2/getajob/static/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/application.py` & `getajob-0.6.2/getajob/test_support/fixtures/application.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/chat.py` & `getajob-0.6.2/getajob/test_support/fixtures/chat.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/company.py` & `getajob-0.6.2/getajob/test_support/fixtures/company.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/recruiter.py` & `getajob-0.6.2/getajob/test_support/fixtures/recruiter.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/recruiter_invitation.py` & `getajob-0.6.2/getajob/test_support/fixtures/recruiter_invitation.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/scheduled_events.py` & `getajob-0.6.2/getajob/test_support/fixtures/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/test_support/fixtures/users.py` & `getajob-0.6.2/getajob/test_support/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/utils.py` & `getajob-0.6.2/getajob/utils.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/algolia/mock.py` & `getajob-0.6.2/getajob/vendor/algolia/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/algolia/models.py` & `getajob-0.6.2/getajob/vendor/algolia/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     company_search = "company_search"
     candidate_search = "candidate_search"
     applicant_search = "applicant_search"
 
 
 class AlgoliaSearchParams(BaseModel):
     query: str | None = None
-    filters: Optional[str] = None   
+    filters: Optional[str] = None
     facet_filters: Optional[str] = None
     attributes_to_retrieve: Optional[str] = None
     page: int = 0
     hits_per_page: int = 10
 
 
 class AlgoliaSearchResults(BaseModel):
```

### Comparing `getajob-0.6.1/getajob/vendor/algolia/repository.py` & `getajob-0.6.2/getajob/vendor/algolia/repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from algoliasearch.search_client import SearchClient
 
 from .client_factory import AlgoliaClientFactory
 from .models import AlgoliaIndex, AlgoliaSearchParams, AlgoliaSearchResults
 
 
 class AlgoliaSearchRepository:
@@ -29,18 +30,20 @@
         return AlgoliaSearchResults(**res)
 
     def get_object(self, object_id: str):
         return self.index.get_object(object_id)
 
     def create_object(self, object_id: str, object_data: dict):
         object_data["objectID"] = object_id
+        object_data = json.loads(json.dumps(object_data, default=str))
         return self.index.save_object(object_data)
 
     def update_object(self, object_id: str, object_data: dict):
         object_data["objectID"] = object_id
+        object_data = json.loads(json.dumps(object_data, default=str))
         return self.index.partial_update_object(object_data)
 
     def partial_update_based_on_attribute(
         self, objects_to_update: list[dict], filter_attribute: str
     ):
         """
         Provide a dictionary of partials updates for objects.
```

### Comparing `getajob-0.6.1/getajob/vendor/clerk/client.py` & `getajob-0.6.2/getajob/vendor/clerk/client.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/companies/models.py` & `getajob-0.6.2/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/companies/repository.py` & `getajob-0.6.2/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/companies/unit_of_work.py` & `getajob-0.6.2/getajob/vendor/clerk/companies/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/mock.py` & `getajob-0.6.2/getajob/vendor/clerk/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.6.2/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.6.2/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.6.2/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.6.2/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/repository.py` & `getajob-0.6.2/getajob/vendor/clerk/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/users/models.py` & `getajob-0.6.2/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/clerk/users/repository.py` & `getajob-0.6.2/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firebase_storage/client_factory.py` & `getajob-0.6.2/getajob/vendor/firebase_storage/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firebase_storage/mock.py` & `getajob-0.6.2/getajob/vendor/firebase_storage/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firebase_storage/repository.py` & `getajob-0.6.2/getajob/vendor/firebase_storage/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firestore/client_factory.py` & `getajob-0.6.2/getajob/vendor/firestore/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firestore/helpers.py` & `getajob-0.6.2/getajob/vendor/firestore/helpers.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firestore/models.py` & `getajob-0.6.2/getajob/vendor/firestore/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/firestore/repository.py` & `getajob-0.6.2/getajob/vendor/firestore/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/kafka/authentication.py` & `getajob-0.6.2/getajob/vendor/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/kafka/client_factory.py` & `getajob-0.6.2/getajob/vendor/kafka/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/kafka/mock.py` & `getajob-0.6.2/getajob/vendor/kafka/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/kafka/models.py` & `getajob-0.6.2/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/kafka/repository.py` & `getajob-0.6.2/getajob/vendor/kafka/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/mailgun/client_factory.py` & `getajob-0.6.2/getajob/vendor/mailgun/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/mailgun/repository.py` & `getajob-0.6.2/getajob/vendor/mailgun/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/openai/mock.py` & `getajob-0.6.2/getajob/vendor/openai/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/openai/repository.py` & `getajob-0.6.2/getajob/vendor/openai/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/openai/settings.py` & `getajob-0.6.2/getajob/vendor/openai/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/getajob/vendor/redis/repository.py` & `getajob-0.6.2/getajob/vendor/redis/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.1/pyproject.toml` & `getajob-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.6.1/PKG-INFO` & `getajob-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

