# openshift.client.UserOpenshiftIoV1Api

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_user_openshift_io_v1_group**](UserOpenshiftIoV1Api.md#create_user_openshift_io_v1_group) | **POST** /apis/user.openshift.io/v1/groups | 
[**create_user_openshift_io_v1_identity**](UserOpenshiftIoV1Api.md#create_user_openshift_io_v1_identity) | **POST** /apis/user.openshift.io/v1/identities | 
[**create_user_openshift_io_v1_user**](UserOpenshiftIoV1Api.md#create_user_openshift_io_v1_user) | **POST** /apis/user.openshift.io/v1/users | 
[**create_user_openshift_io_v1_user_identity_mapping**](UserOpenshiftIoV1Api.md#create_user_openshift_io_v1_user_identity_mapping) | **POST** /apis/user.openshift.io/v1/useridentitymappings | 
[**delete_user_openshift_io_v1_collection_group**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_collection_group) | **DELETE** /apis/user.openshift.io/v1/groups | 
[**delete_user_openshift_io_v1_collection_identity**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_collection_identity) | **DELETE** /apis/user.openshift.io/v1/identities | 
[**delete_user_openshift_io_v1_collection_user**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_collection_user) | **DELETE** /apis/user.openshift.io/v1/users | 
[**delete_user_openshift_io_v1_group**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_group) | **DELETE** /apis/user.openshift.io/v1/groups/{name} | 
[**delete_user_openshift_io_v1_identity**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_identity) | **DELETE** /apis/user.openshift.io/v1/identities/{name} | 
[**delete_user_openshift_io_v1_user**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_user) | **DELETE** /apis/user.openshift.io/v1/users/{name} | 
[**delete_user_openshift_io_v1_user_identity_mapping**](UserOpenshiftIoV1Api.md#delete_user_openshift_io_v1_user_identity_mapping) | **DELETE** /apis/user.openshift.io/v1/useridentitymappings/{name} | 
[**get_user_openshift_io_v1_api_resources**](UserOpenshiftIoV1Api.md#get_user_openshift_io_v1_api_resources) | **GET** /apis/user.openshift.io/v1/ | 
[**list_user_openshift_io_v1_group**](UserOpenshiftIoV1Api.md#list_user_openshift_io_v1_group) | **GET** /apis/user.openshift.io/v1/groups | 
[**list_user_openshift_io_v1_identity**](UserOpenshiftIoV1Api.md#list_user_openshift_io_v1_identity) | **GET** /apis/user.openshift.io/v1/identities | 
[**list_user_openshift_io_v1_user**](UserOpenshiftIoV1Api.md#list_user_openshift_io_v1_user) | **GET** /apis/user.openshift.io/v1/users | 
[**patch_user_openshift_io_v1_group**](UserOpenshiftIoV1Api.md#patch_user_openshift_io_v1_group) | **PATCH** /apis/user.openshift.io/v1/groups/{name} | 
[**patch_user_openshift_io_v1_identity**](UserOpenshiftIoV1Api.md#patch_user_openshift_io_v1_identity) | **PATCH** /apis/user.openshift.io/v1/identities/{name} | 
[**patch_user_openshift_io_v1_user**](UserOpenshiftIoV1Api.md#patch_user_openshift_io_v1_user) | **PATCH** /apis/user.openshift.io/v1/users/{name} | 
[**patch_user_openshift_io_v1_user_identity_mapping**](UserOpenshiftIoV1Api.md#patch_user_openshift_io_v1_user_identity_mapping) | **PATCH** /apis/user.openshift.io/v1/useridentitymappings/{name} | 
[**read_user_openshift_io_v1_group**](UserOpenshiftIoV1Api.md#read_user_openshift_io_v1_group) | **GET** /apis/user.openshift.io/v1/groups/{name} | 
[**read_user_openshift_io_v1_identity**](UserOpenshiftIoV1Api.md#read_user_openshift_io_v1_identity) | **GET** /apis/user.openshift.io/v1/identities/{name} | 
[**read_user_openshift_io_v1_user**](UserOpenshiftIoV1Api.md#read_user_openshift_io_v1_user) | **GET** /apis/user.openshift.io/v1/users/{name} | 
[**read_user_openshift_io_v1_user_identity_mapping**](UserOpenshiftIoV1Api.md#read_user_openshift_io_v1_user_identity_mapping) | **GET** /apis/user.openshift.io/v1/useridentitymappings/{name} | 
[**replace_user_openshift_io_v1_group**](UserOpenshiftIoV1Api.md#replace_user_openshift_io_v1_group) | **PUT** /apis/user.openshift.io/v1/groups/{name} | 
[**replace_user_openshift_io_v1_identity**](UserOpenshiftIoV1Api.md#replace_user_openshift_io_v1_identity) | **PUT** /apis/user.openshift.io/v1/identities/{name} | 
[**replace_user_openshift_io_v1_user**](UserOpenshiftIoV1Api.md#replace_user_openshift_io_v1_user) | **PUT** /apis/user.openshift.io/v1/users/{name} | 
[**replace_user_openshift_io_v1_user_identity_mapping**](UserOpenshiftIoV1Api.md#replace_user_openshift_io_v1_user_identity_mapping) | **PUT** /apis/user.openshift.io/v1/useridentitymappings/{name} | 


# **create_user_openshift_io_v1_group**
> V1Group create_user_openshift_io_v1_group(body, pretty=pretty)



create a Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
body = openshift.client.V1Group() # V1Group | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.create_user_openshift_io_v1_group(body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->create_user_openshift_io_v1_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**V1Group**](V1Group.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1Group**](V1Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_user_openshift_io_v1_identity**
> V1Identity create_user_openshift_io_v1_identity(body, pretty=pretty)



create an Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
body = openshift.client.V1Identity() # V1Identity | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.create_user_openshift_io_v1_identity(body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->create_user_openshift_io_v1_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**V1Identity**](V1Identity.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1Identity**](V1Identity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_user_openshift_io_v1_user**
> V1User create_user_openshift_io_v1_user(body, pretty=pretty)



create an User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
body = openshift.client.V1User() # V1User | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.create_user_openshift_io_v1_user(body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->create_user_openshift_io_v1_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**V1User**](V1User.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1User**](V1User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_user_openshift_io_v1_user_identity_mapping**
> V1UserIdentityMapping create_user_openshift_io_v1_user_identity_mapping(body, pretty=pretty)



create an UserIdentityMapping

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
body = openshift.client.V1UserIdentityMapping() # V1UserIdentityMapping | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.create_user_openshift_io_v1_user_identity_mapping(body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->create_user_openshift_io_v1_user_identity_mapping: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**V1UserIdentityMapping**](V1UserIdentityMapping.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1UserIdentityMapping**](V1UserIdentityMapping.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_collection_group**
> UnversionedStatus delete_user_openshift_io_v1_collection_group(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)



delete collection of Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
field_selector = 'field_selector_example' # str | A selector to restrict the list of returned objects by their fields. Defaults to everything. (optional)
label_selector = 'label_selector_example' # str | A selector to restrict the list of returned objects by their labels. Defaults to everything. (optional)
resource_version = 'resource_version_example' # str | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. (optional)
timeout_seconds = 56 # int | Timeout for the list/watch call. (optional)
watch = true # bool | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_collection_group(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_collection_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **field_selector** | **str**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] 
 **label_selector** | **str**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] 
 **resource_version** | **str**| When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. | [optional] 
 **timeout_seconds** | **int**| Timeout for the list/watch call. | [optional] 
 **watch** | **bool**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_collection_identity**
> UnversionedStatus delete_user_openshift_io_v1_collection_identity(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)



delete collection of Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
field_selector = 'field_selector_example' # str | A selector to restrict the list of returned objects by their fields. Defaults to everything. (optional)
label_selector = 'label_selector_example' # str | A selector to restrict the list of returned objects by their labels. Defaults to everything. (optional)
resource_version = 'resource_version_example' # str | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. (optional)
timeout_seconds = 56 # int | Timeout for the list/watch call. (optional)
watch = true # bool | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_collection_identity(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_collection_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **field_selector** | **str**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] 
 **label_selector** | **str**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] 
 **resource_version** | **str**| When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. | [optional] 
 **timeout_seconds** | **int**| Timeout for the list/watch call. | [optional] 
 **watch** | **bool**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_collection_user**
> UnversionedStatus delete_user_openshift_io_v1_collection_user(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)



delete collection of User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
field_selector = 'field_selector_example' # str | A selector to restrict the list of returned objects by their fields. Defaults to everything. (optional)
label_selector = 'label_selector_example' # str | A selector to restrict the list of returned objects by their labels. Defaults to everything. (optional)
resource_version = 'resource_version_example' # str | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. (optional)
timeout_seconds = 56 # int | Timeout for the list/watch call. (optional)
watch = true # bool | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_collection_user(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_collection_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **field_selector** | **str**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] 
 **label_selector** | **str**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] 
 **resource_version** | **str**| When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. | [optional] 
 **timeout_seconds** | **int**| Timeout for the list/watch call. | [optional] 
 **watch** | **bool**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_group**
> UnversionedStatus delete_user_openshift_io_v1_group(name, body, pretty=pretty, grace_period_seconds=grace_period_seconds, orphan_dependents=orphan_dependents)



delete a Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Group
body = openshift.client.V1DeleteOptions() # V1DeleteOptions | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
grace_period_seconds = 56 # int | The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. (optional)
orphan_dependents = true # bool | Should the dependent objects be orphaned. If true/false, the \"orphan\" finalizer will be added to/removed from the object's finalizers list. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_group(name, body, pretty=pretty, grace_period_seconds=grace_period_seconds, orphan_dependents=orphan_dependents)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Group | 
 **body** | [**V1DeleteOptions**](V1DeleteOptions.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **grace_period_seconds** | **int**| The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. | [optional] 
 **orphan_dependents** | **bool**| Should the dependent objects be orphaned. If true/false, the \&quot;orphan\&quot; finalizer will be added to/removed from the object&#39;s finalizers list. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_identity**
> UnversionedStatus delete_user_openshift_io_v1_identity(name, body, pretty=pretty, grace_period_seconds=grace_period_seconds, orphan_dependents=orphan_dependents)



delete an Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Identity
body = openshift.client.V1DeleteOptions() # V1DeleteOptions | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
grace_period_seconds = 56 # int | The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. (optional)
orphan_dependents = true # bool | Should the dependent objects be orphaned. If true/false, the \"orphan\" finalizer will be added to/removed from the object's finalizers list. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_identity(name, body, pretty=pretty, grace_period_seconds=grace_period_seconds, orphan_dependents=orphan_dependents)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Identity | 
 **body** | [**V1DeleteOptions**](V1DeleteOptions.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **grace_period_seconds** | **int**| The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. | [optional] 
 **orphan_dependents** | **bool**| Should the dependent objects be orphaned. If true/false, the \&quot;orphan\&quot; finalizer will be added to/removed from the object&#39;s finalizers list. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_user**
> UnversionedStatus delete_user_openshift_io_v1_user(name, body, pretty=pretty, grace_period_seconds=grace_period_seconds, orphan_dependents=orphan_dependents)



delete an User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the User
body = openshift.client.V1DeleteOptions() # V1DeleteOptions | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
grace_period_seconds = 56 # int | The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. (optional)
orphan_dependents = true # bool | Should the dependent objects be orphaned. If true/false, the \"orphan\" finalizer will be added to/removed from the object's finalizers list. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_user(name, body, pretty=pretty, grace_period_seconds=grace_period_seconds, orphan_dependents=orphan_dependents)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the User | 
 **body** | [**V1DeleteOptions**](V1DeleteOptions.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **grace_period_seconds** | **int**| The duration in seconds before the object should be deleted. Value must be non-negative integer. The value zero indicates delete immediately. If this value is nil, the default grace period for the specified type will be used. Defaults to a per object value if not specified. zero means delete immediately. | [optional] 
 **orphan_dependents** | **bool**| Should the dependent objects be orphaned. If true/false, the \&quot;orphan\&quot; finalizer will be added to/removed from the object&#39;s finalizers list. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user_openshift_io_v1_user_identity_mapping**
> UnversionedStatus delete_user_openshift_io_v1_user_identity_mapping(name, pretty=pretty)



delete an UserIdentityMapping

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the UserIdentityMapping
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.delete_user_openshift_io_v1_user_identity_mapping(name, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->delete_user_openshift_io_v1_user_identity_mapping: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the UserIdentityMapping | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**UnversionedStatus**](UnversionedStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user_openshift_io_v1_api_resources**
> UnversionedAPIResourceList get_user_openshift_io_v1_api_resources()



get available resources

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()

try: 
    api_response = api_instance.get_user_openshift_io_v1_api_resources()
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->get_user_openshift_io_v1_api_resources: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**UnversionedAPIResourceList**](UnversionedAPIResourceList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/yaml, application/vnd.kubernetes.protobuf
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_openshift_io_v1_group**
> V1GroupList list_user_openshift_io_v1_group(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)



list or watch objects of kind Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
field_selector = 'field_selector_example' # str | A selector to restrict the list of returned objects by their fields. Defaults to everything. (optional)
label_selector = 'label_selector_example' # str | A selector to restrict the list of returned objects by their labels. Defaults to everything. (optional)
resource_version = 'resource_version_example' # str | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. (optional)
timeout_seconds = 56 # int | Timeout for the list/watch call. (optional)
watch = true # bool | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. (optional)

try: 
    api_response = api_instance.list_user_openshift_io_v1_group(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->list_user_openshift_io_v1_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **field_selector** | **str**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] 
 **label_selector** | **str**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] 
 **resource_version** | **str**| When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. | [optional] 
 **timeout_seconds** | **int**| Timeout for the list/watch call. | [optional] 
 **watch** | **bool**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] 

### Return type

[**V1GroupList**](V1GroupList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf, application/json;stream=watch, application/vnd.kubernetes.protobuf;stream=watch

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_openshift_io_v1_identity**
> V1IdentityList list_user_openshift_io_v1_identity(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)



list or watch objects of kind Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
field_selector = 'field_selector_example' # str | A selector to restrict the list of returned objects by their fields. Defaults to everything. (optional)
label_selector = 'label_selector_example' # str | A selector to restrict the list of returned objects by their labels. Defaults to everything. (optional)
resource_version = 'resource_version_example' # str | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. (optional)
timeout_seconds = 56 # int | Timeout for the list/watch call. (optional)
watch = true # bool | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. (optional)

try: 
    api_response = api_instance.list_user_openshift_io_v1_identity(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->list_user_openshift_io_v1_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **field_selector** | **str**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] 
 **label_selector** | **str**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] 
 **resource_version** | **str**| When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. | [optional] 
 **timeout_seconds** | **int**| Timeout for the list/watch call. | [optional] 
 **watch** | **bool**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] 

### Return type

[**V1IdentityList**](V1IdentityList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf, application/json;stream=watch, application/vnd.kubernetes.protobuf;stream=watch

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_user_openshift_io_v1_user**
> V1UserList list_user_openshift_io_v1_user(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)



list or watch objects of kind User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
field_selector = 'field_selector_example' # str | A selector to restrict the list of returned objects by their fields. Defaults to everything. (optional)
label_selector = 'label_selector_example' # str | A selector to restrict the list of returned objects by their labels. Defaults to everything. (optional)
resource_version = 'resource_version_example' # str | When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. (optional)
timeout_seconds = 56 # int | Timeout for the list/watch call. (optional)
watch = true # bool | Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. (optional)

try: 
    api_response = api_instance.list_user_openshift_io_v1_user(pretty=pretty, field_selector=field_selector, label_selector=label_selector, resource_version=resource_version, timeout_seconds=timeout_seconds, watch=watch)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->list_user_openshift_io_v1_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **field_selector** | **str**| A selector to restrict the list of returned objects by their fields. Defaults to everything. | [optional] 
 **label_selector** | **str**| A selector to restrict the list of returned objects by their labels. Defaults to everything. | [optional] 
 **resource_version** | **str**| When specified with a watch call, shows changes that occur after that particular version of a resource. Defaults to changes from the beginning of history. | [optional] 
 **timeout_seconds** | **int**| Timeout for the list/watch call. | [optional] 
 **watch** | **bool**| Watch for changes to the described resources and return them as a stream of add, update, and remove notifications. Specify resourceVersion. | [optional] 

### Return type

[**V1UserList**](V1UserList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf, application/json;stream=watch, application/vnd.kubernetes.protobuf;stream=watch

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_user_openshift_io_v1_group**
> V1Group patch_user_openshift_io_v1_group(name, body, pretty=pretty)



partially update the specified Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Group
body = openshift.client.UnversionedPatch() # UnversionedPatch | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.patch_user_openshift_io_v1_group(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->patch_user_openshift_io_v1_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Group | 
 **body** | [**UnversionedPatch**](UnversionedPatch.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1Group**](V1Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/merge-patch+json, application/strategic-merge-patch+json
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_user_openshift_io_v1_identity**
> V1Identity patch_user_openshift_io_v1_identity(name, body, pretty=pretty)



partially update the specified Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Identity
body = openshift.client.UnversionedPatch() # UnversionedPatch | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.patch_user_openshift_io_v1_identity(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->patch_user_openshift_io_v1_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Identity | 
 **body** | [**UnversionedPatch**](UnversionedPatch.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1Identity**](V1Identity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/merge-patch+json, application/strategic-merge-patch+json
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_user_openshift_io_v1_user**
> V1User patch_user_openshift_io_v1_user(name, body, pretty=pretty)



partially update the specified User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the User
body = openshift.client.UnversionedPatch() # UnversionedPatch | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.patch_user_openshift_io_v1_user(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->patch_user_openshift_io_v1_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the User | 
 **body** | [**UnversionedPatch**](UnversionedPatch.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1User**](V1User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/merge-patch+json, application/strategic-merge-patch+json
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **patch_user_openshift_io_v1_user_identity_mapping**
> V1UserIdentityMapping patch_user_openshift_io_v1_user_identity_mapping(name, body, pretty=pretty)



partially update the specified UserIdentityMapping

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the UserIdentityMapping
body = openshift.client.UnversionedPatch() # UnversionedPatch | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.patch_user_openshift_io_v1_user_identity_mapping(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->patch_user_openshift_io_v1_user_identity_mapping: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the UserIdentityMapping | 
 **body** | [**UnversionedPatch**](UnversionedPatch.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1UserIdentityMapping**](V1UserIdentityMapping.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json-patch+json, application/merge-patch+json, application/strategic-merge-patch+json
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **read_user_openshift_io_v1_group**
> V1Group read_user_openshift_io_v1_group(name, pretty=pretty, exact=exact, export=export)



read the specified Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Group
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
exact = true # bool | Should the export be exact.  Exact export maintains cluster-specific fields like 'Namespace' (optional)
export = true # bool | Should this value be exported.  Export strips fields that a user can not specify. (optional)

try: 
    api_response = api_instance.read_user_openshift_io_v1_group(name, pretty=pretty, exact=exact, export=export)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->read_user_openshift_io_v1_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Group | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **exact** | **bool**| Should the export be exact.  Exact export maintains cluster-specific fields like &#39;Namespace&#39; | [optional] 
 **export** | **bool**| Should this value be exported.  Export strips fields that a user can not specify. | [optional] 

### Return type

[**V1Group**](V1Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **read_user_openshift_io_v1_identity**
> V1Identity read_user_openshift_io_v1_identity(name, pretty=pretty, exact=exact, export=export)



read the specified Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Identity
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
exact = true # bool | Should the export be exact.  Exact export maintains cluster-specific fields like 'Namespace' (optional)
export = true # bool | Should this value be exported.  Export strips fields that a user can not specify. (optional)

try: 
    api_response = api_instance.read_user_openshift_io_v1_identity(name, pretty=pretty, exact=exact, export=export)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->read_user_openshift_io_v1_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Identity | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **exact** | **bool**| Should the export be exact.  Exact export maintains cluster-specific fields like &#39;Namespace&#39; | [optional] 
 **export** | **bool**| Should this value be exported.  Export strips fields that a user can not specify. | [optional] 

### Return type

[**V1Identity**](V1Identity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **read_user_openshift_io_v1_user**
> V1User read_user_openshift_io_v1_user(name, pretty=pretty, exact=exact, export=export)



read the specified User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the User
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)
exact = true # bool | Should the export be exact.  Exact export maintains cluster-specific fields like 'Namespace' (optional)
export = true # bool | Should this value be exported.  Export strips fields that a user can not specify. (optional)

try: 
    api_response = api_instance.read_user_openshift_io_v1_user(name, pretty=pretty, exact=exact, export=export)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->read_user_openshift_io_v1_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the User | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 
 **exact** | **bool**| Should the export be exact.  Exact export maintains cluster-specific fields like &#39;Namespace&#39; | [optional] 
 **export** | **bool**| Should this value be exported.  Export strips fields that a user can not specify. | [optional] 

### Return type

[**V1User**](V1User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **read_user_openshift_io_v1_user_identity_mapping**
> V1UserIdentityMapping read_user_openshift_io_v1_user_identity_mapping(name, pretty=pretty)



read the specified UserIdentityMapping

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the UserIdentityMapping
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.read_user_openshift_io_v1_user_identity_mapping(name, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->read_user_openshift_io_v1_user_identity_mapping: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the UserIdentityMapping | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1UserIdentityMapping**](V1UserIdentityMapping.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_user_openshift_io_v1_group**
> V1Group replace_user_openshift_io_v1_group(name, body, pretty=pretty)



replace the specified Group

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Group
body = openshift.client.V1Group() # V1Group | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.replace_user_openshift_io_v1_group(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->replace_user_openshift_io_v1_group: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Group | 
 **body** | [**V1Group**](V1Group.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1Group**](V1Group.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_user_openshift_io_v1_identity**
> V1Identity replace_user_openshift_io_v1_identity(name, body, pretty=pretty)



replace the specified Identity

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the Identity
body = openshift.client.V1Identity() # V1Identity | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.replace_user_openshift_io_v1_identity(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->replace_user_openshift_io_v1_identity: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the Identity | 
 **body** | [**V1Identity**](V1Identity.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1Identity**](V1Identity.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_user_openshift_io_v1_user**
> V1User replace_user_openshift_io_v1_user(name, body, pretty=pretty)



replace the specified User

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the User
body = openshift.client.V1User() # V1User | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.replace_user_openshift_io_v1_user(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->replace_user_openshift_io_v1_user: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the User | 
 **body** | [**V1User**](V1User.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1User**](V1User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_user_openshift_io_v1_user_identity_mapping**
> V1UserIdentityMapping replace_user_openshift_io_v1_user_identity_mapping(name, body, pretty=pretty)



replace the specified UserIdentityMapping

### Example 
```python
from __future__ import print_statement
import time
import openshift.client
from kubernetes.client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = openshift.client.UserOpenshiftIoV1Api()
name = 'name_example' # str | name of the UserIdentityMapping
body = openshift.client.V1UserIdentityMapping() # V1UserIdentityMapping | 
pretty = 'pretty_example' # str | If 'true', then the output is pretty printed. (optional)

try: 
    api_response = api_instance.replace_user_openshift_io_v1_user_identity_mapping(name, body, pretty=pretty)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserOpenshiftIoV1Api->replace_user_openshift_io_v1_user_identity_mapping: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| name of the UserIdentityMapping | 
 **body** | [**V1UserIdentityMapping**](V1UserIdentityMapping.md)|  | 
 **pretty** | **str**| If &#39;true&#39;, then the output is pretty printed. | [optional] 

### Return type

[**V1UserIdentityMapping**](V1UserIdentityMapping.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: */*
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

