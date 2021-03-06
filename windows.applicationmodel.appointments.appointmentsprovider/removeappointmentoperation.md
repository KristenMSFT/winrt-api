---
-api-id: T:Windows.ApplicationModel.Appointments.AppointmentsProvider.RemoveAppointmentOperation
-api-type: winrt class
---

<!-- Class syntax.
public class RemoveAppointmentOperation : Windows.ApplicationModel.Appointments.AppointmentsProvider.IRemoveAppointmentOperation
-->

# Windows.ApplicationModel.Appointments.AppointmentsProvider.RemoveAppointmentOperation

## -description
Represents the operation object associated with removing an appointment. Appointments provider apps use this info to perform the operation.

## -remarks
This class is used as the value of the [RemoveAppointmentOperation](../windows.applicationmodel.activation/appointmentsproviderremoveappointmentactivatedeventargs_removeappointmentoperation.md) event data property from the [AppointmentsProviderRemoveAppointmentActivatedEventArgs](../windows.applicationmodel.activation/appointmentsproviderremoveappointmentactivatedeventargs.md) event data class. An appointments provider app typically goes through a series of casts and property checks starting from the [IActivatedEventArgs](../windows.applicationmodel.activation/iactivatedeventargs.md) event data of a general activation event handler. If the activation indicates that it's an **AppointmentsProvider** app activation kind with **Remove** as the verb, then it's appropriate to cast event data to [AppointmentsProviderRemoveAppointmentActivatedEventArgs](../windows.applicationmodel.activation/appointmentsproviderremoveappointmentactivatedeventargs.md).

Providers call methods of [RemoveAppointmentOperation](removeappointmentoperation.md) to indicate whether the operation was completed, was canceled, or when a provider error prevented the operation from being completed. Calling these methods influences the async results that the activating app gets back from its [ShowRemoveAppointmentAsync](../windows.applicationmodel.appointments/appointmentmanager_showremoveappointmentasync.md) call. All of the reporting methods ([ReportCompleted](removeappointmentoperation_reportcompleted.md), [ReportCanceled](removeappointmentoperation_reportcanceled.md), [ReportError](removeappointmentoperation_reporterror.md)) dismiss the Remove Appointment UI.

## -examples

## -see-also
## -capabilities
appointmentsSystem
