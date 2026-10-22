Docker mount test

1. Build image `docker build -t incrementor .`
2. Run with mount `docker run --rm --env DATA_PATH=/data/num.txt --mount type=volume,src=incrementor-data,target=/data incrementor` 