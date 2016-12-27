# Alfresco Customize SiteCollaborator Role
According to Alfresco documentation, Share "Collaborators have full rights to the site content that they own; they have rights to edit but not delete content created by other site members". Only Site Manager can delete content regardless ownership. The use case is to enable Site Collaborator to delete content. Since move content = delete in source folder + create in target folder, this also enables Site Collaborator to move content.   

## Solution
Override/extend SiteCollaborator role with added Delete permission. This consists of define & bootstrap of permissionSet and permissionGroup for site.

## Reference
- http://docs.alfresco.com/5.0/references/permissions_share.html
- http://smasue.github.io/add-custom-role
- https://github.com/Alfresco/community-edition/blob/master/projects/repository/config/alfresco/model/sitePermissionDefinitions.xml
- https://github.com/Alfresco/community-edition/blob/master/projects/repository/config/alfresco/model/permissionDefinitions.xml
