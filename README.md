プロジェクトファイルをクローン  

    git clone https://github.com/ryo981/Laravel.git

作業ディレクトリで下記を実行  

    docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php82-composer:latest \
    composer install --ignore-platform-reqs  

.env.exampleを.envにリネームして"vendor/bin/sail up -d"を実行  