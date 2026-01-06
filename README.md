# SAP HANA Connection

Simple Python tool to connect to SAP HANA and pull data into Pandas.

## Setup
1. **VPN**: Connect to your company VPN.
2. **env**: Create an environment file (name it '.env') and fill it in.

## Usage
1. Open db_communication.ipynb in VS Code.
2. Select your Python kernel if needed.
3. Run the cells to load data.

## Troubleshooting

If you see `Connection Refused`:

* **Check VPN:** Ensure your company VPN is connected.
* **Verify Port:** Make sure you are using the **SQL Port** not the WEB port.
* **Refresh Env:** If you changed the `.env` file, **Restart the Jupyter Kernel** to apply changes.
> [!TIP]
> **Test Connection:** Run this in your terminal to check if the port is open:
> ```bash
> telnet <HANA_ADDRESS> <YOUR_PORT>
> ```
> * **If you see a black screen** on the terminal, then it is true and you are connected.
> * **If you see an error 'Connect failed'**, then it is false and you are not connected.
