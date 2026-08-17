# E-Commerce Inventory Dashboard

This is a dynamic inventory dashboard built with JavaServer Pages (JSP) and modern JSTL/EL. It is self-contained without needing raw Java scriptlets for logic.

## How to Run the Project

We are using the Cargo Maven Plugin to launch a local embedded **Tomcat 11** server automatically. You don't need to install or configure Tomcat yourself!

### 1. From the Terminal (Recommended)
Open your terminal at the root of the project (where this `README.md` is located) and run the following command:

```bash
./mvnw clean package cargo:run
```
*(Note: If you are on Windows, use `mvnw.cmd clean package cargo:run` instead).*

### 2. From IntelliJ IDEA
1. Open the **Maven** tool window on the right side of the screen.
2. If you don't see the tasks, click the **Reload All Maven Projects** button.
3. Under your project name, go to **Lifecycle** and double click `clean`, then double click `package`.
4. Then, expand **Plugins** > **cargo** and double-click `cargo:run`.

### 3. From Eclipse IDE
Since this project uses Maven, you can easily import and run it in Eclipse:
1. Open Eclipse and go to **File** > **Import...**
2. Select **Maven** > **Existing Maven Projects** and click **Next**.
3. Browse to the cloned project directory and click **Finish**.
4. Once the project is imported and built, right-click on the `UC-JavaEE` project in the Project Explorer.
5. Select **Run As** > **Run on Server**.
6. Select your configured **Tomcat 11** server and click **Finish**.

*(Alternatively, you can run the Maven goal `clean package cargo:run` directly inside Eclipse via **Run As** > **Maven build...**)*

### Testing the Dashboard
Once the server indicates it has started successfully, open your web browser and go to:
[http://localhost:8080/UC-JavaEE/login.jsp](http://localhost:8080/UC-JavaEE/login.jsp)

**Test Credentials:**
* Username: `admin`
* Password: `111`
