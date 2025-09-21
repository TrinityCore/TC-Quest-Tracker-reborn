TC-Quest-Tracker
================

Quest Tracker is a tool for [TrinityCore](https://github.com/TrinityCore/TrinityCore) that tracks most abandoned quests ([see details](https://github.com/TrinityCore/TrinityCore/pull/13353)). This repository provides a web interface to display tracked quests.

## Prerequisites

- A web server with PHP 8.0+ and MySQL/MariaDB
- [Composer](https://getcomposer.org/) and [Git](https://git-scm.com/) installed

## Enabling Quest Tracker

Enable the Quest Tracker in your **worldserver.conf** file by setting:

```ini
Quests.EnableQuestTracker = 1
```

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/masterking32/TC-Quest-Tracker.git
    ```
2. Navigate to the cloned directory:

    ```bash
    cd TC-Quest-Tracker
    ```

3. In your web server folder, run:

    ```bash
    composer install
    ```

4. Copy and edit **config.php.dist** to set your database connection parameters. Rename it to **config.php**.

5. Ensure the `pdo_mysql` extension is enabled in your `php.ini` file by uncommenting:

    ```
    extension=pdo_mysql
    ```

6. Open your web browser and navigate to the folder where you installed the tracker (e.g., http://localhost/TC-Quest-Tracker).

---

## Screenshots

![Screenshot 1](https://raw.githubusercontent.com/masterking32/TC-Quest-Tracker/refs/heads/main/screenshot1.png)
![Screenshot 2](https://raw.githubusercontent.com/masterking32/TC-Quest-Tracker/refs/heads/main/screenshot2.png)

## License

TC-Quest-Tracker is open-source software licensed under the [GNU AGPL license](https://github.com/masterking32/TC-Quest-Tracker/blob/main/LICENSE).

## Credits

- [masterking32](https://github.com/masterking32)

