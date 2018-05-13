---
swagger: "2.0"
info:
  title: Azure Virtual Network API Check Dns Name Availability
  description: Checks whether a domain name in the cloudapp.net zone is available
    for use.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.Network/locations/{location}/CheckDnsNameAvailability:
    get:
      summary: Check Dns Name Availability
      description: Checks whether a domain name in the cloudapp
      operationId: CheckDnsNameAvailability
      parameters:
      - in: query
        name: domainNameLabel
        description: The domain name to be verified
      - in: path
        name: location
        description: The location of the domain name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - dns name availability
definitions:
  ApplicationGatewayBackendHealth:
    properties:
      backendAddressPools:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendHealthPool:
    properties:
      backendHttpSettingsCollection:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendHealthHttpSettings:
    properties:
      servers:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendHealthServer:
    properties:
      address:
        description: This is a default description.
        type: get
      health:
        description: This is a default description.
        type: get
  ApplicationGatewaySku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
  ApplicationGatewaySslPolicy:
    properties:
      disabledSslProtocols:
        description: This is a default description.
        type: get
  ApplicationGatewayIPConfigurationPropertiesFormat:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayIPConfiguration:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayAuthenticationCertificatePropertiesFormat:
    properties:
      data:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayAuthenticationCertificate:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewaySslCertificatePropertiesFormat:
    properties:
      data:
        description: This is a default description.
        type: get
      password:
        description: This is a default description.
        type: get
      publicCertData:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewaySslCertificate:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayFrontendIPConfigurationPropertiesFormat:
    properties:
      privateIPAddress:
        description: This is a default description.
        type: get
      privateIPAllocationMethod:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayFrontendIPConfiguration:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayFrontendPortPropertiesFormat:
    properties:
      port:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayFrontendPort:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendAddress:
    properties:
      fqdn:
        description: This is a default description.
        type: get
      ipAddress:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendAddressPoolPropertiesFormat:
    properties:
      backendIPConfigurations:
        description: This is a default description.
        type: get
      backendAddresses:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendAddressPool:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendHttpSettingsPropertiesFormat:
    properties:
      port:
        description: This is a default description.
        type: get
      protocol:
        description: This is a default description.
        type: get
      cookieBasedAffinity:
        description: This is a default description.
        type: get
      requestTimeout:
        description: This is a default description.
        type: get
      authenticationCertificates:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayBackendHttpSettings:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayHttpListenerPropertiesFormat:
    properties:
      protocol:
        description: This is a default description.
        type: get
      hostName:
        description: This is a default description.
        type: get
      requireServerNameIndication:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayHttpListener:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayPathRulePropertiesFormat:
    properties:
      paths:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayPathRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayProbePropertiesFormat:
    properties:
      protocol:
        description: This is a default description.
        type: get
      host:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
      interval:
        description: This is a default description.
        type: get
      timeout:
        description: This is a default description.
        type: get
      unhealthyThreshold:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayProbe:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayRequestRoutingRulePropertiesFormat:
    properties:
      ruleType:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayRequestRoutingRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayPropertiesFormat:
    properties:
      operationalState:
        description: This is a default description.
        type: get
      gatewayIPConfigurations:
        description: This is a default description.
        type: get
      authenticationCertificates:
        description: This is a default description.
        type: get
      sslCertificates:
        description: This is a default description.
        type: get
      frontendIPConfigurations:
        description: This is a default description.
        type: get
      frontendPorts:
        description: This is a default description.
        type: get
      probes:
        description: This is a default description.
        type: get
      backendAddressPools:
        description: This is a default description.
        type: get
      backendHttpSettingsCollection:
        description: This is a default description.
        type: get
      httpListeners:
        description: This is a default description.
        type: get
  ApplicationGateway:
    properties:
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ApplicationGatewayUrlPathMapPropertiesFormat:
    properties:
      pathRules:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ApplicationGatewayUrlPathMap:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ApplicationGatewayWebApplicationFirewallConfiguration:
    properties:
      enabled:
        description: This is a default description.
        type: get
      firewallMode:
        description: This is a default description.
        type: get
      ruleSetType:
        description: This is a default description.
        type: get
      ruleSetVersion:
        description: This is a default description.
        type: get
      disabledRuleGroups:
        description: This is a default description.
        type: get
  ApplicationGatewayConnectionDraining:
    properties:
      enabled:
        description: This is a default description.
        type: get
      drainTimeoutInSec:
        description: This is a default description.
        type: get
  ApplicationGatewayFirewallDisabledRuleGroup:
    properties:
      ruleGroupName:
        description: This is a default description.
        type: get
      rules:
        description: This is a default description.
        type: get
  ApplicationGatewayAvailableWafRuleSetsResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ApplicationGatewayFirewallRuleSet:
    properties: []
  ApplicationGatewayFirewallRuleSetPropertiesFormat:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
      ruleSetType:
        description: This is a default description.
        type: get
      ruleSetVersion:
        description: This is a default description.
        type: get
      ruleGroups:
        description: This is a default description.
        type: get
  ApplicationGatewayFirewallRuleGroup:
    properties:
      ruleGroupName:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      rules:
        description: This is a default description.
        type: get
  ApplicationGatewayFirewallRule:
    properties:
      ruleId:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  DnsNameAvailabilityResult:
    properties:
      available:
        description: This is a default description.
        type: get
  AuthorizationPropertiesFormat:
    properties:
      authorizationKey:
        description: This is a default description.
        type: get
      authorizationUseStatus:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ExpressRouteCircuitAuthorization:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  AuthorizationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ExpressRouteCircuitPeeringConfig:
    properties:
      advertisedPublicPrefixes:
        description: This is a default description.
        type: get
      advertisedPublicPrefixesState:
        description: This is a default description.
        type: get
      customerASN:
        description: This is a default description.
        type: get
      routingRegistryName:
        description: This is a default description.
        type: get
  ExpressRouteCircuitStats:
    properties:
      primarybytesIn:
        description: This is a default description.
        type: get
      primarybytesOut:
        description: This is a default description.
        type: get
      secondarybytesIn:
        description: This is a default description.
        type: get
      secondarybytesOut:
        description: This is a default description.
        type: get
  ExpressRouteCircuitPeeringPropertiesFormat:
    properties:
      peeringType:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      azureASN:
        description: This is a default description.
        type: get
      peerASN:
        description: This is a default description.
        type: get
      primaryPeerAddressPrefix:
        description: This is a default description.
        type: get
      secondaryPeerAddressPrefix:
        description: This is a default description.
        type: get
      primaryAzurePort:
        description: This is a default description.
        type: get
      secondaryAzurePort:
        description: This is a default description.
        type: get
      sharedKey:
        description: This is a default description.
        type: get
      vlanId:
        description: This is a default description.
        type: get
  ExpressRouteCircuitPeering:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ExpressRouteCircuitPeeringListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ExpressRouteCircuitSku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      family:
        description: This is a default description.
        type: get
  ExpressRouteCircuitServiceProviderProperties:
    properties:
      serviceProviderName:
        description: This is a default description.
        type: get
      peeringLocation:
        description: This is a default description.
        type: get
      bandwidthInMbps:
        description: This is a default description.
        type: get
  ExpressRouteCircuitPropertiesFormat:
    properties:
      allowClassicOperations:
        description: This is a default description.
        type: get
      circuitProvisioningState:
        description: This is a default description.
        type: get
      serviceProviderProvisioningState:
        description: This is a default description.
        type: get
      authorizations:
        description: This is a default description.
        type: get
      peerings:
        description: This is a default description.
        type: get
      serviceKey:
        description: This is a default description.
        type: get
      serviceProviderNotes:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      gatewayManagerEtag:
        description: This is a default description.
        type: get
  ExpressRouteCircuit:
    properties:
      etag:
        description: This is a default description.
        type: get
  ExpressRouteCircuitArpTable:
    properties:
      age:
        description: This is a default description.
        type: get
      interface:
        description: This is a default description.
        type: get
      ipAddress:
        description: This is a default description.
        type: get
      macAddress:
        description: This is a default description.
        type: get
  ExpressRouteCircuitsArpTableListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ExpressRouteCircuitRoutesTable:
    properties:
      network:
        description: This is a default description.
        type: get
      nextHop:
        description: This is a default description.
        type: get
      locPrf:
        description: This is a default description.
        type: get
      weight:
        description: This is a default description.
        type: get
      path:
        description: This is a default description.
        type: get
  ExpressRouteCircuitsRoutesTableListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ExpressRouteCircuitRoutesTableSummary:
    properties:
      neighbor:
        description: This is a default description.
        type: get
      v:
        description: This is a default description.
        type: get
      as:
        description: This is a default description.
        type: get
      upDown:
        description: This is a default description.
        type: get
      statePfxRcd:
        description: This is a default description.
        type: get
  ExpressRouteCircuitsRoutesTableSummaryListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ExpressRouteCircuitListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ExpressRouteServiceProviderBandwidthsOffered:
    properties:
      offerName:
        description: This is a default description.
        type: get
      valueInMbps:
        description: This is a default description.
        type: get
  ExpressRouteServiceProviderPropertiesFormat:
    properties:
      peeringLocations:
        description: This is a default description.
        type: get
      bandwidthsOffered:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ExpressRouteServiceProvider:
    properties: []
  ExpressRouteServiceProviderListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  FrontendIPConfigurationPropertiesFormat:
    properties:
      inboundNatRules:
        description: This is a default description.
        type: get
      inboundNatPools:
        description: This is a default description.
        type: get
      outboundNatRules:
        description: This is a default description.
        type: get
      loadBalancingRules:
        description: This is a default description.
        type: get
      privateIPAddress:
        description: This is a default description.
        type: get
      privateIPAllocationMethod:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  FrontendIPConfiguration:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  BackendAddressPoolPropertiesFormat:
    properties:
      backendIPConfigurations:
        description: This is a default description.
        type: get
      loadBalancingRules:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  BackendAddressPool:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  LoadBalancingRulePropertiesFormat:
    properties:
      protocol:
        description: This is a default description.
        type: get
      loadDistribution:
        description: This is a default description.
        type: get
      frontendPort:
        description: This is a default description.
        type: get
      backendPort:
        description: This is a default description.
        type: get
      idleTimeoutInMinutes:
        description: This is a default description.
        type: get
      enableFloatingIP:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  LoadBalancingRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  ProbePropertiesFormat:
    properties:
      loadBalancingRules:
        description: This is a default description.
        type: get
      protocol:
        description: This is a default description.
        type: get
      port:
        description: This is a default description.
        type: get
      intervalInSeconds:
        description: This is a default description.
        type: get
      numberOfProbes:
        description: This is a default description.
        type: get
      requestPath:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  Probe:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  InboundNatRulePropertiesFormat:
    properties:
      protocol:
        description: This is a default description.
        type: get
      frontendPort:
        description: This is a default description.
        type: get
      backendPort:
        description: This is a default description.
        type: get
      idleTimeoutInMinutes:
        description: This is a default description.
        type: get
      enableFloatingIP:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  InboundNatRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  InboundNatPoolPropertiesFormat:
    properties:
      protocol:
        description: This is a default description.
        type: get
      frontendPortRangeStart:
        description: This is a default description.
        type: get
      frontendPortRangeEnd:
        description: This is a default description.
        type: get
      backendPort:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  InboundNatPool:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  OutboundNatRulePropertiesFormat:
    properties:
      allocatedOutboundPorts:
        description: This is a default description.
        type: get
      frontendIPConfigurations:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  OutboundNatRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  LoadBalancerPropertiesFormat:
    properties:
      frontendIPConfigurations:
        description: This is a default description.
        type: get
      backendAddressPools:
        description: This is a default description.
        type: get
      loadBalancingRules:
        description: This is a default description.
        type: get
      probes:
        description: This is a default description.
        type: get
      inboundNatRules:
        description: This is a default description.
        type: get
      inboundNatPools:
        description: This is a default description.
        type: get
      outboundNatRules:
        description: This is a default description.
        type: get
      resourceGuid:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  LoadBalancer:
    properties:
      etag:
        description: This is a default description.
        type: get
  LoadBalancerListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ErrorDetails:
    properties: []
  NetworkInterfaceIPConfigurationPropertiesFormat:
    properties:
      applicationGatewayBackendAddressPools:
        description: This is a default description.
        type: post
      loadBalancerBackendAddressPools:
        description: This is a default description.
        type: post
      loadBalancerInboundNatRules:
        description: This is a default description.
        type: post
      privateIPAddress:
        description: This is a default description.
        type: post
      privateIPAllocationMethod:
        description: This is a default description.
        type: post
      privateIPAddressVersion:
        description: This is a default description.
        type: post
      primary:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
  NetworkInterfaceIPConfiguration:
    properties:
      name:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
  NetworkInterfaceDnsSettings:
    properties:
      dnsServers:
        description: This is a default description.
        type: post
      appliedDnsServers:
        description: This is a default description.
        type: post
      internalDnsNameLabel:
        description: This is a default description.
        type: post
      internalFqdn:
        description: This is a default description.
        type: post
      internalDomainNameSuffix:
        description: This is a default description.
        type: post
  NetworkInterfacePropertiesFormat:
    properties:
      ipConfigurations:
        description: This is a default description.
        type: post
      macAddress:
        description: This is a default description.
        type: post
      primary:
        description: This is a default description.
        type: post
      enableAcceleratedNetworking:
        description: This is a default description.
        type: post
      enableIPForwarding:
        description: This is a default description.
        type: post
      resourceGuid:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
  NetworkInterface:
    properties:
      etag:
        description: This is a default description.
        type: post
  NetworkInterfaceListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  EffectiveNetworkSecurityGroup:
    properties:
      effectiveSecurityRules:
        description: This is a default description.
        type: post
  EffectiveNetworkSecurityGroupAssociation:
    properties: []
  EffectiveNetworkSecurityRule:
    properties:
      name:
        description: This is a default description.
        type: post
      protocol:
        description: This is a default description.
        type: post
      sourcePortRange:
        description: This is a default description.
        type: post
      destinationPortRange:
        description: This is a default description.
        type: post
      sourceAddressPrefix:
        description: This is a default description.
        type: post
      destinationAddressPrefix:
        description: This is a default description.
        type: post
      expandedSourceAddressPrefix:
        description: This is a default description.
        type: post
      expandedDestinationAddressPrefix:
        description: This is a default description.
        type: post
      access:
        description: This is a default description.
        type: post
      priority:
        description: This is a default description.
        type: post
  EffectiveNetworkSecurityGroupListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  EffectiveRoute:
    properties:
      name:
        description: This is a default description.
        type: post
      source:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
      addressPrefix:
        description: This is a default description.
        type: post
      nextHopIpAddress:
        description: This is a default description.
        type: post
      nextHopType:
        description: This is a default description.
        type: post
  EffectiveRouteListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  IPConfigurationPropertiesFormat:
    properties:
      privateIPAddress:
        description: This is a default description.
        type: post
      privateIPAllocationMethod:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
  IPConfiguration:
    properties:
      name:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
  SecurityRulePropertiesFormat:
    properties:
      description:
        description: This is a default description.
        type: get
      protocol:
        description: This is a default description.
        type: get
      sourcePortRange:
        description: This is a default description.
        type: get
      destinationPortRange:
        description: This is a default description.
        type: get
      sourceAddressPrefix:
        description: This is a default description.
        type: get
      destinationAddressPrefix:
        description: This is a default description.
        type: get
      access:
        description: This is a default description.
        type: get
      priority:
        description: This is a default description.
        type: get
      direction:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  SecurityRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  SecurityRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  NetworkSecurityGroupPropertiesFormat:
    properties:
      securityRules:
        description: This is a default description.
        type: get
      defaultSecurityRules:
        description: This is a default description.
        type: get
      networkInterfaces:
        description: This is a default description.
        type: get
      subnets:
        description: This is a default description.
        type: get
      resourceGuid:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  NetworkSecurityGroup:
    properties:
      etag:
        description: This is a default description.
        type: get
  NetworkSecurityGroupListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  NetworkWatcher:
    properties:
      etag:
        description: This is a default description.
        type: post
  NetworkWatcherPropertiesFormat:
    properties:
      provisioningState:
        description: This is a default description.
        type: post
  NetworkWatcherListResult:
    properties:
      value:
        description: This is a default description.
        type: post
  TopologyParameters:
    properties:
      targetResourceGroupName:
        description: This is a default description.
        type: post
  Topology:
    properties:
      id:
        description: This is a default description.
        type: post
      createdDateTime:
        description: This is a default description.
        type: post
      lastModified:
        description: This is a default description.
        type: post
      resources:
        description: This is a default description.
        type: post
  TopologyResource:
    properties:
      name:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      associations:
        description: This is a default description.
        type: post
  TopologyAssociation:
    properties:
      name:
        description: This is a default description.
        type: post
      resourceId:
        description: This is a default description.
        type: post
      associationType:
        description: This is a default description.
        type: post
  VerificationIPFlowParameters:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
      direction:
        description: This is a default description.
        type: post
      protocol:
        description: This is a default description.
        type: post
      localPort:
        description: This is a default description.
        type: post
      remotePort:
        description: This is a default description.
        type: post
      localIPAddress:
        description: This is a default description.
        type: post
      remoteIPAddress:
        description: This is a default description.
        type: post
      targetNicResourceId:
        description: This is a default description.
        type: post
  VerificationIPFlowResult:
    properties:
      access:
        description: This is a default description.
        type: post
      ruleName:
        description: This is a default description.
        type: post
  NextHopParameters:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
      sourceIPAddress:
        description: This is a default description.
        type: post
      destinationIPAddress:
        description: This is a default description.
        type: post
      targetNicResourceId:
        description: This is a default description.
        type: post
  NextHopResult:
    properties:
      nextHopType:
        description: This is a default description.
        type: post
      nextHopIpAddress:
        description: This is a default description.
        type: post
      routeTableId:
        description: This is a default description.
        type: post
  SecurityGroupViewParameters:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
  SecurityGroupViewResult:
    properties:
      networkInterfaces:
        description: This is a default description.
        type: post
  SecurityGroupNetworkInterface:
    properties:
      id:
        description: This is a default description.
        type: post
  SecurityRuleAssociations:
    properties:
      defaultSecurityRules:
        description: This is a default description.
        type: post
      effectiveSecurityRules:
        description: This is a default description.
        type: post
  NetworkInterfaceAssociation:
    properties:
      id:
        description: This is a default description.
        type: post
      securityRules:
        description: This is a default description.
        type: post
  SubnetAssociation:
    properties:
      id:
        description: This is a default description.
        type: post
      securityRules:
        description: This is a default description.
        type: post
  PacketCapture:
    properties: []
  PacketCaptureParameters:
    properties:
      target:
        description: This is a default description.
        type: post
      bytesToCapturePerPacket:
        description: This is a default description.
        type: post
      totalBytesPerSession:
        description: This is a default description.
        type: post
      timeLimitInSeconds:
        description: This is a default description.
        type: post
      filters:
        description: This is a default description.
        type: post
  PacketCaptureStorageLocation:
    properties:
      storageId:
        description: This is a default description.
        type: post
      storagePath:
        description: This is a default description.
        type: post
      filePath:
        description: This is a default description.
        type: post
  PacketCaptureFilter:
    properties:
      protocol:
        description: This is a default description.
        type: post
      localIPAddress:
        description: This is a default description.
        type: post
      remoteIPAddress:
        description: This is a default description.
        type: post
      localPort:
        description: This is a default description.
        type: post
      remotePort:
        description: This is a default description.
        type: post
  PacketCaptureListResult:
    properties:
      value:
        description: This is a default description.
        type: post
  PacketCaptureResult:
    properties:
      name:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
  PacketCaptureResultProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: post
  PacketCaptureQueryStatusResult:
    properties:
      name:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      captureStartTime:
        description: This is a default description.
        type: post
      packetCaptureStatus:
        description: This is a default description.
        type: post
      stopReason:
        description: This is a default description.
        type: post
      packetCaptureError:
        description: This is a default description.
        type: post
  TroubleshootingParameters:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
  QueryTroubleshootingParameters:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
  TroubleshootingProperties:
    properties:
      storageId:
        description: This is a default description.
        type: post
      storagePath:
        description: This is a default description.
        type: post
  TroubleshootingResult:
    properties:
      startTime:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      code:
        description: This is a default description.
        type: post
      results:
        description: This is a default description.
        type: post
  TroubleshootingDetails:
    properties:
      id:
        description: This is a default description.
        type: post
      reasonType:
        description: This is a default description.
        type: post
      summary:
        description: This is a default description.
        type: post
      detail:
        description: This is a default description.
        type: post
      recommendedActions:
        description: This is a default description.
        type: post
  TroubleshootingRecommendedActions:
    properties:
      actionId:
        description: This is a default description.
        type: post
      actionText:
        description: This is a default description.
        type: post
      actionUri:
        description: This is a default description.
        type: post
      actionUriText:
        description: This is a default description.
        type: post
  FlowLogProperties:
    properties:
      storageId:
        description: This is a default description.
        type: post
      enabled:
        description: This is a default description.
        type: post
  FlowLogStatusParameters:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
  RetentionPolicyParameters:
    properties:
      days:
        description: This is a default description.
        type: post
      enabled:
        description: This is a default description.
        type: post
  FlowLogInformation:
    properties:
      targetResourceId:
        description: This is a default description.
        type: post
  PublicIPAddressPropertiesFormat:
    properties:
      publicIPAllocationMethod:
        description: This is a default description.
        type: get
      publicIPAddressVersion:
        description: This is a default description.
        type: get
      ipAddress:
        description: This is a default description.
        type: get
      idleTimeoutInMinutes:
        description: This is a default description.
        type: get
      resourceGuid:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  PublicIPAddress:
    properties:
      etag:
        description: This is a default description.
        type: get
  PublicIPAddressListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  PublicIPAddressDnsSettings:
    properties:
      domainNameLabel:
        description: This is a default description.
        type: get
      fqdn:
        description: This is a default description.
        type: get
      reverseFqdn:
        description: This is a default description.
        type: get
  RouteFilterRulePropertiesFormat:
    properties:
      access:
        description: This is a default description.
        type: get
      routeFilterRuleType:
        description: This is a default description.
        type: get
      communities:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  RouteFilterRule:
    properties:
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  PatchRouteFilterRule:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  RouteFilterPropertiesFormat:
    properties:
      rules:
        description: This is a default description.
        type: get
      peerings:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  RouteFilter:
    properties:
      etag:
        description: This is a default description.
        type: get
  PatchRouteFilter:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  RouteFilterListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RouteFilterRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RoutePropertiesFormat:
    properties:
      addressPrefix:
        description: This is a default description.
        type: get
      nextHopType:
        description: This is a default description.
        type: get
      nextHopIpAddress:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  Route:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  RouteTablePropertiesFormat:
    properties:
      routes:
        description: This is a default description.
        type: get
      subnets:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  RouteTable:
    properties:
      etag:
        description: This is a default description.
        type: get
  RouteTableListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RouteListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  BGPCommunity:
    properties:
      serviceSupportedRegion:
        description: This is a default description.
        type: get
      communityName:
        description: This is a default description.
        type: get
      communityValue:
        description: This is a default description.
        type: get
      communityPrefixes:
        description: This is a default description.
        type: get
  BgpServiceCommunityPropertiesFormat:
    properties:
      serviceName:
        description: This is a default description.
        type: get
      bgpCommunities:
        description: This is a default description.
        type: get
  BgpServiceCommunity:
    properties: []
  BgpServiceCommunityListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  UsageName:
    properties:
      value:
        description: This is a default description.
        type: get
      localizedValue:
        description: This is a default description.
        type: get
  Usage:
    properties:
      unit:
        description: This is a default description.
        type: get
      currentValue:
        description: This is a default description.
        type: get
      limit:
        description: This is a default description.
        type: get
  UsagesListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourceNavigationLinkFormat:
    properties:
      linkedResourceType:
        description: This is a default description.
        type: get
      link:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ResourceNavigationLink:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  SubnetPropertiesFormat:
    properties:
      addressPrefix:
        description: This is a default description.
        type: get
      ipConfigurations:
        description: This is a default description.
        type: get
      resourceNavigationLinks:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  VirtualNetworkPeeringPropertiesFormat:
    properties:
      allowVirtualNetworkAccess:
        description: This is a default description.
        type: get
      allowForwardedTraffic:
        description: This is a default description.
        type: get
      allowGatewayTransit:
        description: This is a default description.
        type: get
      useRemoteGateways:
        description: This is a default description.
        type: get
      peeringState:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  Subnet:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  VirtualNetworkPeering:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  SubnetListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  VirtualNetworkPeeringListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  VirtualNetworkPropertiesFormat:
    properties:
      subnets:
        description: This is a default description.
        type: get
      virtualNetworkPeerings:
        description: This is a default description.
        type: get
      resourceGuid:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  VirtualNetwork:
    properties:
      etag:
        description: This is a default description.
        type: get
  VirtualNetworkListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  AddressSpace:
    properties:
      addressPrefixes:
        description: This is a default description.
        type: get
  DhcpOptions:
    properties:
      dnsServers:
        description: This is a default description.
        type: get
  IPAddressAvailabilityResult:
    properties:
      available:
        description: This is a default description.
        type: get
      availableIPAddresses:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayIPConfigurationPropertiesFormat:
    properties:
      privateIPAllocationMethod:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayIPConfiguration:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayPropertiesFormat:
    properties:
      ipConfigurations:
        description: This is a default description.
        type: get
      gatewayType:
        description: This is a default description.
        type: get
      vpnType:
        description: This is a default description.
        type: get
      enableBgp:
        description: This is a default description.
        type: get
      activeActive:
        description: This is a default description.
        type: get
      resourceGuid:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  VpnClientRootCertificatePropertiesFormat:
    properties:
      publicCertData:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  VpnClientRootCertificate:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  VpnClientRevokedCertificatePropertiesFormat:
    properties:
      thumbprint:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  VpnClientRevokedCertificate:
    properties:
      name:
        description: This is a default description.
        type: get
      etag:
        description: This is a default description.
        type: get
  VpnClientConfiguration:
    properties:
      vpnClientRootCertificates:
        description: This is a default description.
        type: get
      vpnClientRevokedCertificates:
        description: This is a default description.
        type: get
  VirtualNetworkGatewaySku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      capacity:
        description: This is a default description.
        type: get
  BgpSettings:
    properties:
      asn:
        description: This is a default description.
        type: get
      bgpPeeringAddress:
        description: This is a default description.
        type: get
      peerWeight:
        description: This is a default description.
        type: get
  BgpPeerStatus:
    properties:
      localAddress:
        description: This is a default description.
        type: get
      neighbor:
        description: This is a default description.
        type: get
      asn:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      connectedDuration:
        description: This is a default description.
        type: get
      routesReceived:
        description: This is a default description.
        type: get
      messagesSent:
        description: This is a default description.
        type: get
      messagesReceived:
        description: This is a default description.
        type: get
  GatewayRoute:
    properties:
      localAddress:
        description: This is a default description.
        type: get
      network:
        description: This is a default description.
        type: get
      nextHop:
        description: This is a default description.
        type: get
      sourcePeer:
        description: This is a default description.
        type: get
      origin:
        description: This is a default description.
        type: get
      asPath:
        description: This is a default description.
        type: get
      weight:
        description: This is a default description.
        type: get
  VirtualNetworkGateway:
    properties:
      etag:
        description: This is a default description.
        type: get
  VpnClientParameters:
    properties:
      processorArchitecture:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  BgpPeerStatusListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  GatewayRouteListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  TunnelConnectionHealth:
    properties:
      tunnel:
        description: This is a default description.
        type: get
      connectionStatus:
        description: This is a default description.
        type: get
      ingressBytesTransferred:
        description: This is a default description.
        type: get
      egressBytesTransferred:
        description: This is a default description.
        type: get
      lastConnectionEstablishedUtcTime:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayConnectionPropertiesFormat:
    properties:
      authorizationKey:
        description: This is a default description.
        type: get
      connectionType:
        description: This is a default description.
        type: get
      routingWeight:
        description: This is a default description.
        type: get
      sharedKey:
        description: This is a default description.
        type: get
      connectionStatus:
        description: This is a default description.
        type: get
      tunnelConnectionStatus:
        description: This is a default description.
        type: get
      egressBytesTransferred:
        description: This is a default description.
        type: get
      ingressBytesTransferred:
        description: This is a default description.
        type: get
      enableBgp:
        description: This is a default description.
        type: get
      usePolicyBasedTrafficSelectors:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayConnection:
    properties:
      etag:
        description: This is a default description.
        type: get
  VirtualNetworkGatewayConnectionListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ConnectionResetSharedKey:
    properties:
      keyLength:
        description: This is a default description.
        type: get
  ConnectionSharedKey:
    properties:
      value:
        description: This is a default description.
        type: get
  IpsecPolicy:
    properties:
      saLifeTimeSeconds:
        description: This is a default description.
        type: get
      saDataSizeKilobytes:
        description: This is a default description.
        type: get
      ipsecEncryption:
        description: This is a default description.
        type: get
      ipsecIntegrity:
        description: This is a default description.
        type: get
      ikeEncryption:
        description: This is a default description.
        type: get
      ikeIntegrity:
        description: This is a default description.
        type: get
      dhGroup:
        description: This is a default description.
        type: get
      pfsGroup:
        description: This is a default description.
        type: get
  LocalNetworkGatewayPropertiesFormat:
    properties:
      gatewayIpAddress:
        description: This is a default description.
        type: get
      resourceGuid:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  LocalNetworkGateway:
    properties:
      etag:
        description: This is a default description.
        type: get
  LocalNetworkGatewayListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
x-collection-name: Azure Virtual Network
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---