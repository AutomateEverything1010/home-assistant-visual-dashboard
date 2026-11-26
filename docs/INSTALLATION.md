# Installation

1. Back up your existing dashboard before editing it.
2. Install the custom cards and theme listed in the repository README.
3. Copy the contents of this repository’s `assets/` folder into your Home Assistant `/config/www/assets/` directory. If you use Samba Share, open the Home Assistant share from Finder and copy the folder there.
4. In Home Assistant, open **Settings → Dashboards**, create a dashboard (or open an existing one in raw configuration mode), and import/paste `dashboard.yaml`.
5. Replace all `replace_me_*` entity IDs and `YOUR_HA_USERNAME` using `docs/ENTITY-MAPPING.md`.
6. Confirm that the referenced scripts, helpers, buttons, climate entity, lights, and switches exist in your instance. If not, adapt those actions to your own devices.
7. Check the browser console and Home Assistant logs for missing resources or entity IDs, then test each control.

## Asset paths

The YAML uses `/local/assets/...` paths. Home Assistant serves files in `/config/www/` under `/local/`, so preserve the `assets` subfolder name.

## Important

This is a dashboard configuration, not a complete Home Assistant backup or a plug-and-play integration. It does not create entities, helpers, scripts, automations, integrations, or custom-card resources for you.
