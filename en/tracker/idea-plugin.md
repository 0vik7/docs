# Plugin for the **IntelliJ** IDE

If you're using an IDE from JetBrains, integrate it with {{ tracker-name }} using the [plugin](https://plugins.jetbrains.com/plugin/10549-yandex-tracker-integration). The plugin allows you to work with issues directly from the IDE. Learn  more about the plugin's features in the Help for your IDE: [IntelliJ IDEA](https://www.jetbrains.com/help/idea/managing-tasks-and-context.html), [PhpStorm](https://www.jetbrains.com/help/phpstorm/2017.2/managing-tasks-and-contexts.html), [WebStorm](https://www.jetbrains.com/help/webstorm/managing-tasks-and-context.html), [PyCharm](https://www.jetbrains.com/help/pycharm/managing-tasks-and-context.html), [RubyMine](https://www.jetbrains.com/help/ruby/managing-tasks-and-context.html), [AppCode](https://www.jetbrains.com/help/objc/managing-tasks-and-context.html), [CLion](https://www.jetbrains.com/help/clion/managing-tasks-and-context.html), [GoLand](https://www.jetbrains.com/help/clion/2017.2/managing-tasks-and-contexts.html), [DataGrip](https://www.jetbrains.com/help/idea/managing-tasks-and-context.html), [Rider](https://www.jetbrains.com/help/rider/managing_tasks_and_context.html), [MPS](https://www.jetbrains.com/help/idea/managing-tasks-and-context.html), and [Android Studio](https://www.jetbrains.com/help/idea/managing-tasks-and-context.html).

{% note warning %}

The plugin only allows you to work with issues that you are assigned to.

{% endnote %}

## Install the plugin {#section_jm1_r4d_kdb}


#### From the repository

1. Open the settings window in IntelliJ: **File** → **Settings**.

1. On the **Plugins** tab, click **Browse Repositories**.

1. In the search bar, enter `Yandex Tracker integration`.

1. Click **Install** on the right side of the window.

1. Restart your IDE.

#### From a file

1. Download the plugin from the official [plugin marketplace](https://plugins.jetbrains.com/plugin/10549-yandex-tracker-integration).

1. Open the settings window in IntelliJ: **File** → **Settings**.

1. On the **Plugins** tab, click **Install plugin from disk**.

1. Specify the location of the archive with the plugin and click **OK**.

1. Restart your IDE.

## Connect the plugin to {{ tracker-name }} {#section_vgn_cqd_kdb}


To make the plugin work, link it to your account:


1. Log in to {{ tracker-name }}.

1. Launch your IntelliJ IDE and select **Tools** → **Tasks & Contexts** → **Configure Servers**.

1. Click **+** and select **Yandex Tracker**.

1. Click **Authorize** and wait for the browser window to appear.

1.  Grant access to your data on Yandex for the <q>Yandex Tracker IntelliJ Plugin</q>.

1. Copy the authentication code.

1. Paste the code into the **Authentication Code** window in the IDE.

1. Click **OK**.

1. Select the queue that you want to work in.

1. Click **OK**.


[Contact support](troubleshooting.md)

