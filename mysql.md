# MySQL

## Add a user

    mysql -uroot
    > GRANT ALL PRIVILEGES ON $db.$table TO '$username[@$host]' IDENTIFIED BY '$password';
    > FLUSH PRIVILEGES;

## Delete a user

    mysql -uroot
    > DELETE FROM user WHERE user='$username';
