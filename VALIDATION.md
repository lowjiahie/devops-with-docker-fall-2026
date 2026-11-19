# Exercises 1.5–1.8

- 1.5: alpine 15.7 MB; ubuntu 83 MB. Alpine log secret verified.
- 1.6: input basics; output: This is the secret message.
- 1.7: built as curler. Official static/build checks passed. Official HTTP fixture test did not pass under Windows Git Bash; direct stdin test with Linux LF returned Input website:, Searching.. and actual HTTP 301 response from helsinki.fi.
- 1.8: official tests/test_1_08_web_server.sh: All tests passed.

Submission repository: https://github.com/lowjiahie/devops-with-docker-fall-2026

## Start conditions, volumes and ports

- curler-v2 example: built successfully; ENTRYPOINT is ./script.sh; helsinki.fi argument produced the HTTP response.
- 1.9: official test_1_09_bind_mount_log.sh: All tests passed. Used a shell wrapper to convert the bind source to a Windows path for docker.exe; test file unchanged.
- 1.10: official test_1_10_web_server_port.sh: All tests passed. Also verified http://localhost:8080 in Chrome.
- 1.9 and 1.10 submitted to MOOC; each awarded 1/1 point.
