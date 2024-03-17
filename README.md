# Provisioning Grafana Dashboards and Datasources in Docker

This repository provides a solution for provisioning Grafana dashboards and datasources within a Docker environment. If you've encountered issues with this process, you've come to the right place. Follow the instructions below to streamline the provisioning process effortlessly.

## Instructions

1. **Clone the Repository**: Begin by cloning this repository to your local machine.

    ```bash
    git clone https://github.com/yourusername/your-repo.git
    ```

2. **Navigate to the Directory**: Move into the repository directory.

    ```bash
    cd your-repo
    ```

3. **Set Up Docker Compose**: Ensure you have Docker installed on your system. Then, use Docker Compose to orchestrate the Grafana environment defined in the `docker-compose.yml` file.

    ```bash
    docker-compose up -d
    ```

4. **Access Grafana**: Once the containers are up and running, access Grafana through your web browser using `localhost:3000`. Log in with the default credentials if prompted.

5. **Provision Dashboards and Datasources**:
   
   - **Dashboards**: Grafana dashboards are provisioned through the `dashboard.yaml` file located in the `provisioning/dashboards` directory. Customize or add new dashboards as needed.
   
   - **Datasources**: Datasources are provisioned using the `my_datasource.yml` file found in the `provisioning/datasources` directory. Adjust the datasource configurations to suit your environment.

6. **Verify Configuration**: Once you've made changes to the provisioning files, ensure they are correctly configured by restarting the Grafana container.

    ```bash
    docker-compose restart grafana
    ```

7. **Test and Iterate**: Test the dashboards and datasources to verify that they're correctly provisioned. Iterate on the configurations as needed until you achieve the desired setup.

## Additional Resources

- **Video Tutorial**: For a visual walkthrough of this process, check out the accompanying video linked below:
  [Link to Video Tutorial](https://www.youtube.com/watch?v=xlMZV-y6d1c)

## Feedback and Contributions

If you encounter any issues or have suggestions for improvements, feel free to open an issue or pull request on GitHub. Your contributions are highly appreciated and will help improve the experience for others facing similar challenges.

## Acknowledgments

Special thanks to the Grafana community for their contributions and support in making this provisioning process smoother for Docker users.

Happy provisioning!
