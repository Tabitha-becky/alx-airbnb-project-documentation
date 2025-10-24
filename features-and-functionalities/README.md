# 🏡 Airbnb Clone Backend Features and Functionalities

This document outlines the key features and functionalities of the Airbnb Clone backend system. The project focuses on designing and implementing a robust backend that supports all major Airbnb-like operations including user management, property listings, bookings, and payments.

---

## 🔑 Key Features

### 1. User Management
- User registration, login, and authentication
- Profile updates and password reset
- Role-based access (User, Host, Admin)

### 2. Property Management
- Add, edit, and delete property listings
- Upload property images and descriptions
- Manage availability and pricing

### 3. Booking System
- Search for properties based on filters
- Reserve and cancel bookings
- Track booking history and status

### 4. Payment Processing
- Secure payment integration
- Automatic receipt generation
- Refund and cancellation management

### 5. Review and Rating
- Users can leave reviews for properties
- Display average ratings for listings
- Handle report or flag options

### 6. Admin Dashboard
- Manage users, bookings, and properties
- Generate analytical reports
- Handle customer disputes and issues

---

## 🖼️ Features Diagram
Below is the visual representation of the backend features and how they interact.


[Airbnb Clone Backend.drawio](https://github.com/user-attachments/files/23114896/Airbnb.Clone.Backend.drawio)
<mxfile host="app.diagrams.net" agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/141.0.0.0 Safari/537.36 Edg/141.0.0.0" version="28.2.8" pages="3">
  <diagram name="Page-1" id="jT0niZTb2vt1gDhTfXFk">
    <mxGraphModel dx="997" dy="1582" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="850" pageHeight="1100" background="light-dark(#000000,#000000)" math="0" shadow="1">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-1" value="id(PK)&lt;div&gt;name&lt;/div&gt;&lt;div&gt;email&lt;/div&gt;&lt;div&gt;password&lt;/div&gt;&lt;div&gt;role&lt;/div&gt;" style="rounded=0;whiteSpace=wrap;html=1;labelBackgroundColor=none;fillColor=#FFE45E;strokeColor=#FF6392;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="210" y="-20" width="120" height="80" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-3" value="id(PK)&lt;div&gt;user_id(FK)&lt;/div&gt;&lt;div&gt;title&lt;/div&gt;&lt;div&gt;location&lt;/div&gt;&lt;div&gt;price per night&lt;/div&gt;&lt;div&gt;&lt;br&gt;&lt;/div&gt;" style="rounded=0;whiteSpace=wrap;html=1;labelBackgroundColor=none;fillColor=#FFE45E;strokeColor=#FF6392;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="10" y="150" width="130" height="100" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-5" value="id(PK)&lt;div&gt;booking_(FK)&lt;/div&gt;&lt;div&gt;amount&lt;/div&gt;&lt;div&gt;status&lt;/div&gt;&lt;div&gt;payment_date&lt;/div&gt;" style="rounded=0;whiteSpace=wrap;html=1;labelBackgroundColor=none;fillColor=#FFE45E;strokeColor=#FF6392;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="212" y="530" width="160" height="120" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-6" value="id(PK)&lt;div&gt;user_id(FK)&lt;/div&gt;&lt;div&gt;property_id(FK)&lt;/div&gt;&lt;div&gt;rating&lt;/div&gt;&lt;div&gt;comment&lt;/div&gt;" style="rounded=0;whiteSpace=wrap;html=1;labelBackgroundColor=none;fillColor=#FFE45E;strokeColor=#FF6392;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="210" y="290" width="130" height="120" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-8" value="Property" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="30" y="120" width="110" height="30" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-9" value="Review" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="225" y="270" width="80" height="20" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-11" value="Booking" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="420" y="110" width="90" height="30" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-12" value="Payment" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="260" y="500" width="45" height="30" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-13" value="User" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="240" y="-50" width="60" height="30" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-16" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;exitX=0.411;exitY=0.2;exitDx=0;exitDy=0;exitPerimeter=0;entryX=1.017;entryY=0.35;entryDx=0;entryDy=0;entryPerimeter=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" source="uABQ2NIdkwBAP7M8gCmg-11" target="uABQ2NIdkwBAP7M8gCmg-1" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="452.04" y="110" as="sourcePoint" />
            <mxPoint x="340" y="30" as="targetPoint" />
            <Array as="points">
              <mxPoint x="400" y="70" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-18" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="200" y="360" as="sourcePoint" />
            <mxPoint x="90" y="260" as="targetPoint" />
            <Array as="points" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-19" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;exitX=1;exitY=0.5;exitDx=0;exitDy=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" source="uABQ2NIdkwBAP7M8gCmg-4" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="440" y="250" as="sourcePoint" />
            <mxPoint x="490" y="200" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-20" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;entryX=0.477;entryY=1.058;entryDx=0;entryDy=0;entryPerimeter=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" target="uABQ2NIdkwBAP7M8gCmg-4" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="350" y="370" as="sourcePoint" />
            <mxPoint x="490" y="200" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-4" value="&lt;br&gt;&lt;div&gt;id(PK)&lt;/div&gt;&lt;div&gt;user_id(FK)&lt;/div&gt;&lt;div&gt;property_id(FK)&lt;br&gt;start_date&lt;/div&gt;&lt;div&gt;end_date&lt;/div&gt;" style="rounded=0;whiteSpace=wrap;html=1;labelBackgroundColor=none;fillColor=#FFE45E;strokeColor=#FF6392;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="400" y="140" width="130" height="120" as="geometry" />
        </mxCell>
        <mxCell id="uABQ2NIdkwBAP7M8gCmg-28" value="" style="endArrow=none;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;exitX=0.5;exitY=0;exitDx=0;exitDy=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" source="uABQ2NIdkwBAP7M8gCmg-12" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="260" y="500" as="sourcePoint" />
            <mxPoint x="280" y="420" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-4" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;exitX=0.391;exitY=0.233;exitDx=0;exitDy=0;exitPerimeter=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" source="uABQ2NIdkwBAP7M8gCmg-8" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="110" y="100" as="sourcePoint" />
            <mxPoint x="210" y="10" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-5" value="1 to many" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="40" y="40" width="80" height="30" as="geometry" />
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-6" value="1 to many" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="400" y="40" width="110" height="30" as="geometry" />
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-7" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;exitX=1;exitY=0.5;exitDx=0;exitDy=0;entryX=0;entryY=0.5;entryDx=0;entryDy=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" source="a89ZV-lxXhtlrsjyx7Gi-8" target="uABQ2NIdkwBAP7M8gCmg-4" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="300" y="250" as="sourcePoint" />
            <mxPoint x="350" y="200" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-9" value="" style="endArrow=none;dashed=1;html=1;rounded=0;fontSize=12;startSize=8;endSize=8;curved=1;exitX=1;exitY=0.5;exitDx=0;exitDy=0;entryX=0;entryY=0.5;entryDx=0;entryDy=0;labelBackgroundColor=none;fontColor=default;strokeColor=#FF6392;" parent="1" source="uABQ2NIdkwBAP7M8gCmg-3" target="a89ZV-lxXhtlrsjyx7Gi-8" edge="1">
          <mxGeometry width="50" height="50" relative="1" as="geometry">
            <mxPoint x="140" y="200" as="sourcePoint" />
            <mxPoint x="400" y="200" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-8" value="1 to many" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="210" y="185" width="110" height="30" as="geometry" />
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-10" value="1 to many" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="70" y="300" width="60" height="30" as="geometry" />
        </mxCell>
        <mxCell id="a89ZV-lxXhtlrsjyx7Gi-11" value="1 to 1" style="text;html=1;whiteSpace=wrap;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;rounded=0;fontSize=16;labelBackgroundColor=none;fontColor=#5AA9E6;" parent="1" vertex="1">
          <mxGeometry x="400" y="320" width="60" height="30" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
  <diagram id="9hoaBf60TuPUc6PpFXlC" name="Page-2">
    <mxGraphModel dx="778" dy="934" grid="0" gridSize="10" guides="0" tooltips="1" connect="0" arrows="0" fold="1" page="0" pageScale="1" pageWidth="850" pageHeight="1100" background="light-dark(#000000,#000000)" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-2" value="User Authentication - Register - Login - Logout" style="rounded=1;whiteSpace=wrap;fillColor=#cfe2f3;" vertex="1" parent="1">
          <mxGeometry x="100" y="150" width="160" height="100" as="geometry" />
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-3" value="Property Management - Add Listing - Edit Listing - Delete Listing" style="rounded=1;whiteSpace=wrap;fillColor=#d9ead3;" vertex="1" parent="1">
          <mxGeometry x="300" y="150" width="160" height="100" as="geometry" />
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-4" value="Booking System - Create Booking - View Booking - Cancel Booking" style="rounded=1;whiteSpace=wrap;fillColor=#f9cb9c;" vertex="1" parent="1">
          <mxGeometry x="500" y="150" width="160" height="100" as="geometry" />
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-5" value="Payments - Process Payment - Refund" style="rounded=1;whiteSpace=wrap;fillColor=#ffe599;" vertex="1" parent="1">
          <mxGeometry x="200" y="300" width="160" height="80" as="geometry" />
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-6" value="Reviews - Add Review - View Review" style="rounded=1;whiteSpace=wrap;fillColor=#ead1dc;" vertex="1" parent="1">
          <mxGeometry x="400" y="300" width="160" height="80" as="geometry" />
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-7" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" source="24Mp7nH3qYo_fXe5TfXF-1" target="24Mp7nH3qYo_fXe5TfXF-2">
          <mxGeometry relative="1" as="geometry">
            <Array as="points">
              <mxPoint x="180" y="16" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-8" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;exitX=0.486;exitY=0.718;exitDx=0;exitDy=0;exitPerimeter=0;" edge="1" parent="1" source="24Mp7nH3qYo_fXe5TfXF-1" target="24Mp7nH3qYo_fXe5TfXF-3">
          <mxGeometry relative="1" as="geometry">
            <Array as="points">
              <mxPoint x="370" y="62" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-9" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" source="24Mp7nH3qYo_fXe5TfXF-1" target="24Mp7nH3qYo_fXe5TfXF-4">
          <mxGeometry relative="1" as="geometry">
            <Array as="points">
              <mxPoint x="580" y="17" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-14" value="" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="24Mp7nH3qYo_fXe5TfXF-1">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="382" y="35" as="sourcePoint" />
            <mxPoint x="191" y="140" as="targetPoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="24Mp7nH3qYo_fXe5TfXF-1" value="User" style="shape=umlActor;verticalLabelPosition=bottom;verticalAlign=top;" vertex="1" parent="1">
          <mxGeometry x="334" y="-25" width="72" height="120" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
  <diagram id="4ZHlJd4QUT3MYEiTrx8j" name="Page-3">
    <mxGraphModel dx="1417" dy="934" grid="0" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="0" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <mxCell id="XFdQAgroeFoa6A09mows-3" value="Register Account" style="ellipse;whiteSpace=wrap;fillColor=#cfe2f3;" vertex="1" parent="1">
          <mxGeometry x="150" y="50" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-4" value="Login / Logout" style="ellipse;whiteSpace=wrap;fillColor=#cfe2f3;" vertex="1" parent="1">
          <mxGeometry x="150" y="150" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-5" value="Add / Edit / Delete Property" style="ellipse;whiteSpace=wrap;fillColor=#d9ead3;" vertex="1" parent="1">
          <mxGeometry x="350" y="50" width="160" height="60" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-6" value="Create / View / Cancel Booking" style="ellipse;whiteSpace=wrap;fillColor=#f9cb9c;" vertex="1" parent="1">
          <mxGeometry x="350" y="150" width="160" height="60" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-7" value="Process Payments / Refunds" style="ellipse;whiteSpace=wrap;fillColor=#ffe599;" vertex="1" parent="1">
          <mxGeometry x="550" y="150" width="160" height="60" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-8" value="Add / View Reviews" style="ellipse;whiteSpace=wrap;fillColor=#ead1dc;" vertex="1" parent="1">
          <mxGeometry x="550" y="50" width="160" height="60" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-9" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-3">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="96" y="129" as="sourcePoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-10" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-4">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="96" y="129" as="sourcePoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-11" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-5">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="96" y="129" as="sourcePoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-12" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-6">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="96" y="129" as="sourcePoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-13" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-7">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="96" y="129" as="sourcePoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-15" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-5">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="698" y="-23" as="sourcePoint" />
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-16" style="edgeStyle=orthogonalEdgeStyle;endArrow=classic;" edge="1" parent="1" target="XFdQAgroeFoa6A09mows-7">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="757" y="33" as="sourcePoint" />
            <Array as="points">
              <mxPoint x="738" y="33" />
              <mxPoint x="772" y="33" />
              <mxPoint x="772" y="180" />
            </Array>
          </mxGeometry>
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-18" value="user" style="ellipse;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="-27" y="94" width="120" height="80" as="geometry" />
        </mxCell>
        <mxCell id="XFdQAgroeFoa6A09mows-22" value="admin" style="ellipse;whiteSpace=wrap;html=1;" vertex="1" parent="1">
          <mxGeometry x="697" y="-51" width="120" height="80" as="geometry" />
        </mxCell>
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
